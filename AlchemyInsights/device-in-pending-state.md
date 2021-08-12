---
title: Zařízení ve stavu čeká na vyřízení
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
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53913996"
---
# <a name="device-in-pending-state"></a>Zařízení ve stavu čeká na vyřízení

**Předpoklady:**

1. Pokud registrace zařízení nastavujete poprvé, ujistěte se prosím, že jste si prohlédli Úvod ke správě zařízení v [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) který vás provede tím, jak získat zařízení pod kontrolou Azure AD.
2. Pokud přímo zaregistrujete zařízení do Azure AD a zaregistrujete je do Intune, budete [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) muset zajistit, že jste nakonfigurovali [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) a měli jste licenci na prvním místě.
3. Ujistěte se, že máte oprávnění provádět operace v Azure AD a místní službě AD. Nastavení pro registrace zařízení může spravovat jenom globální správce v Azure AD. Pokud navíc nastavujete automatické registrace v místní službě Active Directory, musíte být správcem služby Active Directory a služby AD FS (pokud je to možné).

Proces registrace hybridního připojení k Azure AD vyžaduje, aby zařízení byla v podnikové síti. Funguje taky přes VPN, ale k tomu existují určité upozornění. Vyslyšeli jsme zákazníky, kteří potřebují pomoc s řešením potíží s hybridním procesem registrace připojení k Azure AD za vzdálených pracovních podmínek.

**Cloudové ověřovací prostředí (pomocí synchronizace hodnot hash hesel Azure AD nebo předávkovací ověřování)**

Tento registrační tok se taky označuje jako "Synchronizovat spojení".

Tady je přehled toho, co se stane během procesu registrace:

1. Windows 10 zjistí záznam spojovacího bodu služby (SCP), když se uživatel přihlásí k zařízení.

    1. Zařízení se nejdřív pokusí načíst informace o tenantovi ze SCP na straně klienta v registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Další informace najdete v [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Pokud se to nepodaří, zařízení komunikuje s místní službou Active Directory, aby se informace o tenantovi z SCP dostaly. Pokud chcete ověřit SCP, přečtěte si tento [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Doporučujeme povolit SCP ve službě Active Directory a k počátečnímu ověření používat jenom SCP na straně klienta.

2. Windows 10 se snaží komunikovat s Azure AD v kontextu systému a ověřit se v Azure AD.

    Pokud má zařízení přístup k prostředkům Microsoftu pod systémovým účtem, můžete ověřit pomocí skriptu [Test Device Registration Connectivity](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 certifikát podepsaný svým držitelem a uloží ho pod objekt počítače v místní službě Active Directory. To vyžaduje viditelnost na řadiči domény.

4. Objekt zařízení s certifikátem se synchronizuje s Azure AD přes Azure AD Připojení. Cyklus synchronizace je ve výchozím nastavení každých 30 minut, ale závisí na konfiguraci služby Azure AD Připojení. Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. V této fázi byste měli mít možnost zobrazit předmět zařízení ve **stavu** Čeká se na vyřízení v části Device blade (Zařízení) na portálu Azure Portal.

6. Při příštím přihlášení uživatele k Windows 10 se registrace dokončí.

    > [!NOTE]
    > Pokud používáte VPN a odhlášení/přihlášení ukončí připojení domény, můžete registraci spustit ručně. To můžete udělat takhle:
    >
    > `dsregcmd /join`Vyděste místně výzvu správce nebo vzdáleně přes PSExec do počítače.
    >
    > Příklad: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Běžné problémy s registrací Azure Active Directory zařízení najdete v článku [Nejčastější dotazy k zařízením.](https://docs.microsoft.com/azure/active-directory/devices/faq)
