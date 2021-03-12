---
title: Office se nedaří aktivovat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704923"
---
# <a name="unable-to-activate-office"></a>Office se nedaří aktivovat

- Zkontrolujte, jestli platnost vašeho předplatného vypršela.
- Ujistěte se, že máte předplatné, které umožňuje klientské licence, jako je Office 365 Business nebo Business Premium, a ověřte, že má [uživatel přiřazenou licenci.](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide)
- Zkontrolujte, jestli je uživatel přihlášený k Office pomocí stejného účtu, který má přiřazenou licenci.
- Podívejte se na [stránku stavu služeb Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) a zjistěte, jestli se vyskytly nějaké problémy.
- Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru, jestli neblokují aplikace Microsoft 365 a přístup k internetu. Přečtěte si [Adresy URL a rozsahy IP adres pro Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Adresy URL a rozsahy IP adres pro Office 365").

**Tip** Na počítačích s Windows za vás můžeme diagnostikovat a automaticky vyřešit několik běžných problémů s přihlášením k Office. Pokud chcete používat náš automatizovaný nástroj, stáhněte si a spusťte nástroj **[Microsoft Support and Recovery Assistant.](https://aka.ms/SaRA-OfficeSignInScenario)**

Při řešení problémů postupujte takto:

- Otevřete aplikaci Office a [odhlaste se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) od všech existujících uživatelských účtů. [Odeberte](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) a [znovu přiřaďte](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licence Office, a potom [se přihlaste k Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocí ovlivněného uživatelského účtu.
- Spusťte [Poradce při potížích s aktivací](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Resetujte stav aktivace Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Obnovení stavu aktivace Office").
- [Proveďte online opravu Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA).

Další řešení problémů najdete tady:  

- [Chyby typu Nelicencovaný produkt a chyby aktivace v Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Chyba „Je nám líto, ale nemůžeme se připojit k vašemu účtu. Zkuste to prosím znovu později.“ při aktivaci Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)