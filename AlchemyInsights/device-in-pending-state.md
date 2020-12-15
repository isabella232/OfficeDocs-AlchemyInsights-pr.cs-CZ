---
title: Zařízení čeká na vyřízení.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/11/2020
ms.locfileid: "49677572"
---
# <a name="device-in-pending-state"></a>Zařízení čeká na vyřízení.

**Požadovaných**

1. Pokud zadáváte registrace zařízení poprvé, ujistěte se, že jste provedli kontrolu nad [správou zařízení v Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , která vás seznámí s postupem, jak získat zařízení pod kontrolou Azure AD.
2. Pokud zaregistrujete zařízení do Azure AD přímo a zapíšete je do Intune, budete muset zajistit, že jste [nakonfigurovali](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) v Intune, a budete mít nejdřív [licenci](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .
3. Zkontrolujte, jestli máte oprávnění provádět operace v Azure AD a místním AD. Jenom globální správce Azure AD může spravovat nastavení pro registrace zařízení. Pokud navíc nastavujete automatické registrace v místní službě Active Directory, budete muset být správcem služby Active Directory a AD FS (Pokud je to možné).

Proces registrace hybridního služby Azure AD vyžaduje, aby zařízení byla v podnikové síti. Funguje to taky přes VPN, ale je to jen to. Všichni vyslechní zákazníci, kteří potřebují pomoct s odstraňováním potíží se službou hybridního připojení Azure AD v části vzdálené práce.

**Prostředí pro ověřování v cloudu (pomocí algoritmu hash synchronizace nebo předávacího ověřování v Azure AD)**

Tento registrační tok se označuje také jako "synchronizační spojení".

Tady je přehled toho, co se děje během registrace:

1. Windows 10 vyhledá záznam spojovacího bodu služby, když se uživatel přihlásí do zařízení.

    1. Zařízení se nejprve pokusí načíst informace o tenantovi ze služby SCP na straně klienta v registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Další informace najdete v tématu [Document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Pokud selže, zařízení komunikuje s místní službou Active Directory, aby získala informace o tenantovi ze služby SCP. Pokud chcete ověřit spojovací bod služby, přečtěte si tento [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Doporučujeme, abyste v adresáři Active Directory povolili spojovací bod služby a aby se při počátečním ověřování používaly spojovací bod služby.

2. Ve Windows 10 se pokoušíte komunikovat s Azure AD v kontextu systému, abyste se ověřili vůči službě Azure AD.

    Můžete ověřit, jestli má zařízení přístup k prostředkům společnosti Microsoft pod účtem System pomocí skriptu pro [připojení k testování registrace zařízení](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 generuje certifikát podepsaný svým držitelem a uloží ho pod objektem počítače v místním adresáři Active Directory. To vyžaduje, aby řadič domény promohl.

4. Objekt zařízení, který má certifikát, se synchronizuje s Azure AD přes Azure AD Connect. Cyklus synchronizace je ve výchozím nastavení každých 30 minut, ale závisí na konfiguraci služby Azure AD Connect. Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. V této fázi by mělo být v části zařízení na portálu Azure Portal zobrazeno zařízení s předmětem "**čeká**".

6. Při příštím přihlášení uživatele k Windows 10 bude registrace dokončena.

    > [!NOTE]
    > Pokud používáte připojení k síti VPN, může být aktivace aktivována ručně a odhlášením nebo přihlášením ukončuje připojení domény. Postup:
    >
    > Dejte mu na `dsregcmd /join` počítači lokálně výzvu nebo vzdáleně přes PsExec.
    >
    > Například: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Běžné problémy s registrací zařízení Azure Active Directory najdete v tématu [Časté otázky k zařízení](https://docs.microsoft.com/azure/active-directory/devices/faq).
