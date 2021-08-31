---
title: Problémy s přihlášením k Microsoft 365 aplikacím
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744629"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problémy s přihlášením Microsoft 365 Apps

Poznámka: Pokud používáte starší verzi Windows (například Windows 7 SP1, Windows Server 2008 R2), použijte [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) snadnou opravu k povolení protokolu TLS 1.2 jako výchozího. Další informace najdete v článku Aktualizace a povolení [tls 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)jako výchozích zabezpečených protokolů ve WinHTTP v Windows .

Pokud chcete vyřešit problémy s přihlášením Microsoft 365, vyzkoušejte na příslušném počítači následující možnosti:  

- Další Windows najdete v Recommendations řešení běžných problémů s [přihlášením.](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Mac najdete v [tématu Nemůžu se přihlásit k Office 2016 pro Mac aplikaci](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Tip** Na Windows počítačích můžeme diagnostikovat a automaticky vyřešit několik běžných Office problémy s přihlášením. Stáhněte si a spusťte **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** a použijte náš automatizovaný nástroj.

**Poznámka:** Zakázání moderního ověřování (ADAL) nebo správy webových účtů (WAM) pro řešení problémů s přihlášením nebo **aktivací se nedoporučuje.** Pokud dojde k chybám při připojování Microsoft 365 pomocí Office 2013, ujistěte se, že pro klienta Office ověřování. [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Konkrétní akce řešení potíží najdete v těchto článku:

[Problémy s připojením při přihlášení po aktualizaci Office 2016 build 16.0.7967 ve Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Nemůžete se přihlásit ke svému účtu organizace, jako je Office 365, Azure nebo Intune.](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Řešení potíží s aplikacemi mimo prohlížeč, které se neschytá přihlásit k Office 365, Azure nebo Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Opakovaně se v aplikaci Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)