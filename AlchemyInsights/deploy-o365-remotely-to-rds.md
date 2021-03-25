---
title: Nasazení aplikací Microsoft 365 pro podniky pro sdílené použití na RDS, Terminálovém serveru nebo VDI
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200666"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Nasazení aplikací Microsoft 365 pro podniky pro sdílené použití na RDS, Terminálovém serveru nebo VDI

Nasazení aplikací Microsoft 365 pro podniky pomocí služby Vzdálená plocha (RDS), dříve s názvem Terminálová služba:

- Musíte mít plán Microsoft 365 pro firmy nebo plán Office 365, který zahrnuje Aplikace Microsoft 365 pro podniky, jako je Office 365 Enterprise E3 nebo Enterprise E5.
   > [!NOTE]
   > Plány Microsoft 365 Apps pro firmy a Microsoft 365 Business Standard nezahrnují Aplikace Microsoft 365 pro podniky.
- Musíte povolit [aktivaci sdíleného počítače](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Můžete si taky stáhnout a spustit [Pomocníka pro](https://aka.ms/SaRA_OfficeSCA_M365Portal) podporu a obnovení Microsoftu a nainstalovat aplikace Microsoft 365 pro podniky v režimu aktivace sdíleného počítače.

Další informace o předpokladech, pokynech k instalaci a pokynech k přizpůsobené instalaci pomocí Nástroje pro nasazení Office najdete v tématu Nasazení [aplikací Microsoft 365 pro](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)podniky pomocí služby Vzdálená plocha .

Oprava chyb týkajících se aktivace sdíleného počítače:

- Podívejte [se na článek Řešení problémů s aktivací sdíleného počítače pro Aplikace Microsoft 365 pro podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Přečtěte si téma zaměřené na [resetování stavu aktivace Microsoft 365 Apps pro podniky](https://go.microsoft.com/fwlink/?linkid=2109218).

Pokud chcete nainstalovat Microsoft 365 Apps pro podniky na RDS z Centra pro správu Microsoftu 365, které používá výchozí nastavení instalace , postupujte takto:

1. Zkontrolujte, jaké máte předplatné. [Zjistěte, jak](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)na to.
2. V případě potřeby přepněte na jiné předplatné. [Zjistěte, jak](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)na to.
3. Pokud je Office už nainstalovaný na serveru RDS pomocí jiných předplatných Microsoftu, odinstalujte ho. Například tak, že v **Ovládacích panelech**  >  **odinstalujete program**. Pokud máte problémy, odinstalujte ji pomocí nástroje Microsoft Support and [Recovery Assistant.](https://aka.ms/SARA-OfficeUninstall-Alchemy)
4. Na serveru RDS se přihlaste do Centra pro správu Microsoftu 365 pomocí účtu správce a [nainstalujte aplikace Microsoft 365 pro podniky](https://portal.office.com/OLS/MySoftware.aspx).
5. Po instalaci Office ***se neotev ít ani*** se přihlásit k žádným aplikacím Office.
6. Na serveru RDS povolte aktivaci sdíleného počítače úpravou registru takto:
   1. Klikněte pravým tlačítkem myši na tlačítko Windows v levém dolním rohu obrazovky a vyberte **Spustit.** Do pole Otevřít zadejte příkaz **regedit**, a potom vyberte **OK**.
   2. Po **zobrazení** výzvy k povolení editoru registru k provedení změn ve vašem zařízení vyberte Ano.
   3. V Editoru registru přidejte řetězcovou hodnotu **SharedComputerLicensing** s nastavením 1 v části HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na serveru RDS se přihlaste jako koncový ***uživatel a*** ověřte, jestli je pro Aplikace [Microsoft 365 pro podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)povolená aktivace sdíleného počítače.
