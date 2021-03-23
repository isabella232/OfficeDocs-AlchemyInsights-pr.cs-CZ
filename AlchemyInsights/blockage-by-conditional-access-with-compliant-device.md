---
title: Podmíněný přístup mi zablokuje zařízení kompatibilní se standardem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035058"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Podmíněný přístup mi zablokuje zařízení kompatibilní se standardem

**Vysoce doporučené nástroje**

- [Nástroj Poradce při potížích s registrací zařízení](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – komplexní nástroj, který pomáhá řešit nejčastější problémy s registrací zařízení.
- [Skript Připojení k registraci testovacího zařízení](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – nástroj, který slouží k zajištění přístupu zařízení k koncovým bodům registrace zařízení pod systémovým účtem.
- [Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) – nástroj používaný k hledání a správě zastaralých zařízení ve vašem prostředí.

Tady jsou některé běžné důvody, proč u zařízení kompatibilního s předpisy  může dojít k selhání podmíněného přístupu nebo k tomu, proč se uživatelům může při přihlašování k prostředku organizace zobrazit zpráva.

1. **Zařízení není v požadovaném stavu zařízení s MDM:**

Ověřte, že je zařízení zaregistrované u schváleného poskytovatele MDM, jako je Intune, a *označí se jako kompatibilní*. Další informace o Intune najdete v tomto [dokumentu.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Pokud chcete lépe porozumět dodržování předpisů zařízení a Intune, podívejte se na informace v tématu Použití zásad dodržování předpisů k nastavení pravidel pro zařízení, [která spravujete v Intune.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Pokud máte problémy s registrací zařízení v Intune, najděte podrobnosti o řešení potíží v článku Řešení potíží [s registrací zařízení v Microsoftu.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Pokud chcete další podporu Intune, vytvořte žádost o podporu. Pokud to chcete udělat, navštivte stránku Nápověda a [podpora Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Zařízení není připojené k síti organizací:**

Aby bylo možné získat přístup k prostředkům organizace, musí být zařízení připojené k síti organizace, a to buď prostřednictvím přímého připojení, nebo virtuální privátní sítě (VPN) a také připojené k místní nebo Azure Active Directory. Informace o připojení pracovního zařízení k síti organizace najdete v tématu Připojení pracovního zařízení k [síti vaší organizace.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Pokud chcete zaregistrovat osobní zařízení nebo zařízení BYOD, podívejte se na článek Registrace osobního zařízení v [síti vaší organizace](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Pokud chcete ověřit, jestli se zařízení připojilo k síti, postupujte podle pokynů pro registrovaná zařízení [tady](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) nebo pracovní [zařízení tady](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Pokud chcete problém vyřešit s připojením k síti Organizace, postupujte podle následujících pokynů:

    1. Přihlaste se k Windows pomocí pracovního nebo školního účtu, například pomocí alain@contoso.com.
    2. Připojte se k síti vaší organizace přes VPN nebo DirectAccess.
    3. Po připojení zařízení zamknete stisknutím **klávesy s logem Windows+L.**
    4. Odemkněte zařízení pomocí pracovního nebo školního účtu a zkuste se k problematické aplikaci nebo službě znovu dostat.

Pokud se zobrazí **chybová zpráva Nemůžete** se tam znovu dostat, problém je pravděpodobně jinde.

3. **Operační systém není podporovaný:**

Ujistěte se, že používáte podporovanou verzi operačního systému, včetně těchto:

- **Klient Windows**: Windows 7 nebo novější

- **Windows Server:** Windows Server 2008 R2 nebo novější

- **macOS**: macOS X nebo novější

- **Android a iOS:** Nejnovější verze mobilních operačních systémů s Androidem a iOS

4. **Webový prohlížeč není podporovaný:**

Níže najdete podporované prohlížeče. Pro podporu Chromu ve Windows 1703 nebo novějších verzích je potřeba rozšíření Účtů Windows 10. U Edge 85+ musí být uživatel přihlášený, aby správně předal informace o dodržování předpisů zařízení. Další podrobnosti najdete [tady.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS:** Microsoft Edge, prohlížeč spravovaný Intune, Safari
- **Android**: **Microsoft Edge**: Prohlížeč spravovaný Intune, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2:** Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Tady najdete další informace **o tom, jak se k** této zprávě nemůžete dostat a jak vyřešit [potíže.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
