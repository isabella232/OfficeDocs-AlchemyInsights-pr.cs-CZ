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
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330952"
---
# <a name="troubleshoot-prt-issue"></a>Poradce při potížích s PRT

Aby se ověření dokončilo na libovolném zařízení, musí být plně zaregistrované a v dobrém stavu a musí být schopné získat token primární aktualizace (PRT).

Proces registrace hybridního připojení k Azure AD vyžaduje, aby zařízení byla v podnikové síti. Funguje taky přes VPN, ale k tomu existují určité upozornění. Vyslyšeli jsme zákazníky, kteří potřebují pomoc s řešením potíží s procesem registrace hybridního připojení k Azure AD za okolností vzdálené práce. Tady je přehled toho, co se děje "pod kapotou" během procesu registrace.

**Cloudové ověřovací prostředí (pomocí synchronizace hodnot hash hesel Azure AD nebo předávkovací ověřování)**

Tento registrační tok se taky označuje jako "Synchronizovat spojení".

1. Windows 10 zjistí záznam SCP po přihlášení uživatele k zařízení.
    1. Zařízení se nejdřív pokusí načíst informace o tenantovi z klienta SCP v registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Pokud se to nepodaří, zařízení komunikuje s místní službou Active Directory (AD), aby se informace o tenantovi dostaly z spojovacího bodu služby (SCP). Pokud chcete ověřit SCP, přečtěte si prosím tento [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

**Poznámka:** Doporučujeme povolit SCP ve službě AD a k počátečnímu ověření používat jenom SCP na straně klienta.

2. Windows 10 se snaží komunikovat s Azure AD v kontextu systému a ověřit se v Azure AD. Pomocí skriptu Připojení k registraci testovacího zařízení můžete ověřit, jestli má zařízení přístup k prostředkům Microsoftu pod systémovým účtem.

3. Windows 10 certifikát podepsaný svým držitelem a uloží ho pod objekt počítače v místní službě AD. To vyžaduje viditelnost na řadiči domény.

4. Objekt zařízení, který má certifikát, se synchronizuje s Azure AD přes Azure AD Připojení. Cyklus synchronizace je ve výchozím nastavení každých 30 minut, ale závisí na konfiguraci služby Azure AD Připojení. Další informace najdete v tomto [dokumentu.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. V této fázi byste měli mít možnost zobrazit předmět zařízení ve stavu Čeká se na vyřízení v části Device blade (Zařízení) na portálu Azure Portal.

6. Při příštím přihlášení uživatele k Windows 10 se registrace dokončí. 

**Poznámka:** Pokud používáte VPN a proces odhlášení ukončí připojení domény, můžete registraci spustit ručně:
 1. Vyděste dsregcmd /join místně na výzvu správce nebo vzdáleně přes PSExec do počítače. Například PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Další podrobnosti o problémech s hybridním připojením najdete v tématu [Řešení potíží se zařízeními.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
