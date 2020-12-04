---
title: Poradce při potížích s PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573379"
---
# <a name="troubleshoot-prt-issue"></a>Poradce při potížích s PRT

Aby jakékoli zařízení mohlo dokončit získání ověření, musí být plně registrováno a v dobrém stavu a může získat primární obnovovací token (PRT).

Proces registrace hybridního služby Azure AD vyžaduje, aby zařízení byla v podnikové síti. Funguje to taky přes VPN, ale je to jen to. Podíváme se, že zákazníci potřebují pomoct s odstraňováním potíží se službou hybridního připojení Azure AD v rámci podmínek vzdálené práce. Tady je přehled toho, co se děje "pod digestoří" během procesu registrace.

**Prostředí pro ověřování v cloudu (pomocí algoritmu hash synchronizace nebo předávacího ověřování v Azure AD)**

Tento registrační tok se označuje také jako "synchronizační spojení".

1. Windows 10 zjistí záznam SCP na přihlášení uživatele k zařízení.
    1. Zařízení se nejprve pokusí načíst informace o tenantovi ze služby SCP na straně klienta v registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Pokud selže, zařízení komunikuje se službou místní služby Active Directory (AD), aby získala informace o tenantovi od spojovacího bodu služby (SCP). Pokud chcete ověřit spojovací bod služby, podívejte se na tento [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Doporučujeme v reklamě povolit spojovací bod služby a k počátečnímu ověření jenom používat spojovací bod služby.

2. Ve Windows 10 se pokoušíte komunikovat s Azure AD v kontextu systému, abyste se ověřili vůči službě Azure AD. Můžete ověřit, jestli má zařízení přístup k prostředkům společnosti Microsoft pod účtem System pomocí skriptu pro připojení k testování registrace zařízení.

3. Windows 10 generuje certifikát podepsaný svým držitelem a uloží ho pod objektem počítače v místním AD. To vyžaduje, aby řadič domény promohl.

4. Objekt zařízení, který má certifikát, se synchronizuje s Azure AD přes Azure AD Connect. Cyklus synchronizace je ve výchozím nastavení každých 30 minut, ale závisí na konfiguraci služby Azure AD Connect. Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. V této fázi by mělo být v části zařízení na portálu Azure Portal zobrazeno zařízení s předmětem "čeká".

6. Při příštím přihlášení uživatele k Windows 10 bude registrace dokončena. 

> [!NOTE]
> Pokud používáte připojení k síti VPN a proces přihlašování se odhlášením ukončí připojení k doméně, můžete ručně spustit registraci:
 1. Dejte dsregcmd/JOIN místně ve výzvě pro správu nebo vzdáleně přes PSExec na PC. Například PsExec-s \\ win10client01 cmd, dsregcmd/JOIN

 2. Další informace o problémech s hybridním připojením najdete v článku [řešení potíží se zařízeními](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
