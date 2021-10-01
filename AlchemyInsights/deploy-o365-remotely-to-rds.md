---
title: Nasazení Microsoft 365 Apps pro sdílené použití na rds, terminálový server nebo VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077243"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Nasazení Microsoft 365 Apps pro sdílené použití na rds, terminálový server nebo VDI

Pokud chcete Microsoft 365 Apps vzdálenou plochu (RDS), dříve Terminálovou službou, musíte:

- Pokud používáte starší verzi Windows (například Windows 7 SP1, Windows Server 2008 R2), použijte snadnou opravu. Snadná oprava a další informace najdete v článku Aktualizace, která povolí [protokoly TLS 1.1 a TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)jako výchozí zabezpečené protokoly ve WinHTTP v Windows . 
- Máte plán, který zahrnuje Microsoft 365 Apps pro velké organizace (dříve Office 365 Plus). Například Office 365 E3 nebo Microsoft 365 E5 nebo jakýkoli plán, který zahrnuje desktopovou verzi Project nebo Visio, například Project Plan 3 nebo Visio Plan 2, nebo plán Microsoft 365 Business Premium, který zahrnuje také Microsoft 365 Apps pro firmy.
- Povolte aktivaci sdíleného počítače. Další informace najdete v tématu [Přehled aktivace sdíleného počítače pro Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Poznámka:** Pokud chcete nainstalovat Microsoft 365 Apps v režimu aktivace sdíleného počítače, stáhněte a spusťte [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal). Podrobnosti o předpokladech, pokynech k instalaci a pokynech k přizpůsobení instalací pomocí nástroje pro nasazení Office najdete v tématu Nasazení Microsoft 365 Apps pomocí služby [Vzdálená plocha](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services).

Pokud chcete opravit chyby související s aktivací sdíleného počítače, podívejte se na tyto informace:

- [Řešení problémů s aktivací sdíleného počítače pro Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Resetování stavu aktivace Microsoft 365 Apps pro podniky.](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Pokud chcete nainstalovat Microsoft 365 Apps rds z Centrum pro správu Microsoftu 365, který používá výchozí nastavení instalace, postupujte takto:

1. Zkontrolujte, Microsoft 365 máte plán. Další informace najdete v tématu [Jaké předplatné mám?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. V případě potřeby přepněte na jiný Microsoft 365 plán. Další informace najdete v tématu [Upgrade na jiný plán](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. Pokud Microsoft 365 Apps server RDS nainstalovaný pomocí jiných nekompatibilních plánů, odinstalujte ho tak, že v Ovládacích panelech   >  **odinstalujete program**. Pokud na problémy naběháte, odinstalujte ho tak, že si [stáhnete Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. Na serveru RDS se přihlaste k účtu Centrum pro správu Microsoftu 365 správce a [nainstalujte si Office](https://portal.office.com/OLS/MySoftware.aspx).

   Po Office instalace se neotev ít nebo se přihlásit k žádným Office aplikacím.

1. Na serveru RDS povolte aktivaci sdíleného počítače úpravou registru:

   1. Klikněte pravým tlačítkem na Windows v levém dolním rohu obrazovky a vyberte **Spustit.** Do pole Otevřít zadejte příkaz **regedit**, a potom vyberte **OK**.

   1. Po zobrazení výzvy, aby Editor registru umožnil provádět změny ve vašem zařízení, vyberte **Ano**.

   1. V Editoru registru přidejte v části HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration řetězcovou hodnotu **SharedComputerLicensing** s nastavením **1** .

1. Na serveru RDS se přihlaste jako koncový uživatel a ověřte, jestli je pro tento počítač povolená Microsoft 365 Apps. 

   Podrobnosti najdete v tématu [Ověření, jestli je](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)povolená aktivace sdíleného počítače pro Microsoft 365 Apps .