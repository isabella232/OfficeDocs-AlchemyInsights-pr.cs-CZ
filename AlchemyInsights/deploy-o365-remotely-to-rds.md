---
title: Nasazení Microsoft 365 Apps pro velké organizace pro sdílené použití v rds, terminálovém serveru nebo VDI
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
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031471"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Nasazení Microsoft 365 Apps pro velké organizace pro sdílené použití v rds, terminálovém serveru nebo VDI

Nasazení služby Microsoft 365 Apps pro velké organizace vzdálené plochy (RDS), dříve pojmenované Terminálová služba:

- Musíte mít plán Microsoft 365 for Business nebo plán Office 365, který zahrnuje Microsoft 365 Apps pro velké organizace, například Office 365 Enterprise E3 nebo Enterprise E5.
   > [!NOTE]
   > Plány Microsoft 365 Apps pro firmy a Microsoft 365 Business Standard plány nezahrnují Microsoft 365 Apps pro velké organizace.
- Musíte povolit [aktivaci sdíleného počítače](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Můžete si taky stáhnout a spustit [microsoftový Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) a nainstalovat Microsoft 365 Apps pro velké organizace v režimu aktivace sdíleného počítače.

Další informace o předpokladech, pokynech k instalaci a pokynech k přizpůsobené instalaci pomocí nástroje pro nasazení Office najdete v tématu Nasazení Microsoft 365 Apps pro velké organizace pomocí služby [Vzdálená plocha](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Oprava chyb týkajících se aktivace sdíleného počítače:

- Další informace najdete v tématu Řešení problémů s aktivací [sdíleného Microsoft 365 Apps pro velké organizace](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Přečtěte si téma zaměřené na [resetování stavu aktivace Microsoft 365 Apps pro podniky](https://go.microsoft.com/fwlink/?linkid=2109218).

Pokud chcete nainstalovat Microsoft 365 Apps pro velké organizace rds z Centrum pro správu Microsoftu 365, který používá výchozí nastavení ***instalace***, postupujte takto:

1. Zkontrolujte, jaké máte předplatné. [Zjistěte, jak](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)na to.
2. V případě potřeby přepněte na jiné předplatné. [Zjistěte, jak](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)na to.
3. Pokud Office server RDS nainstalovaný pomocí jiných předplatných Microsoftu, odinstalujte ho. Například tak, že v **Ovládacích panelech**  >  **odinstalujete program**. Pokud máte [problémy, Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) microsoftu odinstalovat.
4. Na serveru RDS se přihlaste k účtu Centrum pro správu Microsoftu 365 správce a [nainstalujte si Microsoft 365 Apps pro velké organizace](https://portal.office.com/OLS/MySoftware.aspx).
5. Po Office se ***neotev ít*** ani se k žádným aplikacím Office přihlásit.
6. Na serveru RDS povolte aktivaci sdíleného počítače úpravou registru takto:
   1. Klikněte pravým tlačítkem na Windows v levém dolním rohu obrazovky a vyberte **Spustit.** Do pole Otevřít zadejte příkaz **regedit**, a potom vyberte **OK**.
   2. Po **zobrazení** výzvy k povolení editoru registru k provedení změn ve vašem zařízení vyberte Ano.
   3. V Editoru registru přidejte řetězcovou hodnotu **SharedComputerLicensing** s nastavením 1 v části HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na serveru RDS se přihlaste jako koncový ***uživatel a*** ověřte, že je povolená aktivace sdíleného počítače [pro Microsoft 365 Apps pro velké organizace](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
