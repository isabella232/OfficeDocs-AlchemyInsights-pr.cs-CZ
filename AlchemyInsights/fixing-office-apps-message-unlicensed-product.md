---
title: Nelze aktivovat Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9a33b7880aff6016ef6df88960d6f59ac9dd50382c7e99d72ca36bc3c9f344ea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928362"
---
# <a name="unable-to-activate-office"></a>Nelze aktivovat Office

**Poznámka:** Pokud používáte starší verzi Windows (například Windows 7), ujistěte se, že je jako výchozí povolená tls 1.2. Další informace najdete v článku Aktualizace a povolení [tls 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)jako výchozích zabezpečených protokolů ve WinHTTP v Windows .

- Zkontrolujte, jestli platnost vašeho předplatného vypršela.
- Ujistěte se, že máte předplatné, které umožňuje klientské licence, například Office 365 Business nebo obchodní Premium, a zkontrolujte, jestli má [uživatel přiřazenou licenci.](/microsoft-365/admin/manage/assign-licenses-to-users)
- Zkontrolujte, jestli je uživatel přihlášený k Office pomocí stejného účtu, který má přiřazenou licenci.
- Podívejte se na [stránku stavu služeb Office 365](/office365/enterprise/view-service-health) a zjistěte, jestli se vyskytly nějaké problémy.
- Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, že Microsoft 365 aplikace neblokují přístup k internetu. Přečtěte si [Adresy URL a rozsahy IP adres pro Office 365](/office365/enterprise/urls-and-ip-address-ranges "Rozsahy adres IP a URL Office 365.").

**Tip** Na Windows počítačích můžeme diagnostikovat a automaticky opravit několik běžných problémů Office přihlášení. Stáhněte si a spusťte **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** a použijte náš automatizovaný nástroj.

Při řešení problémů postupujte takto:

- Otevřete aplikaci Office a [odhlaste se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) od všech existujících uživatelských účtů. [Odeberte](/microsoft-365/admin/manage/remove-licenses-from-users) a [znovu přiřaďte](/microsoft-365/admin/manage/assign-licenses-to-users) licence Office, a potom [se přihlaste k Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocí ovlivněného uživatelského účtu.
- Spusťte [Poradce při potížích s aktivací](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Resetujte stav aktivace Office](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Obnovení Office stavu aktivace").
- [Proveďte online opravu Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA).

Další řešení problémů najdete tady:  

- [Chyby typu Nelicencovaný produkt a chyby aktivace v Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Chyba „Je nám líto, ale nemůžeme se připojit k vašemu účtu. Zkuste to prosím znovu později.“ při aktivaci Office](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)