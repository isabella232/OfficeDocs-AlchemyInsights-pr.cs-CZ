---
title: Nasazení aplikací Microsoft 365 pro podnik pro sdílení pro sdílené použití na RDS, terminálovém serveru nebo VDI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786270"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Nasazení aplikací Microsoft 365 pro podnik pro sdílení pro sdílené použití na RDS, terminálovém serveru nebo VDI

Nasazení aplikací Microsoft 365 pro podnik pomocí služby Vzdálená plocha (RDS) s názvem Terminálová služba
- Musíte mít plán Microsoft 365 pro firmy nebo plán Office 365, který zahrnuje aplikace Microsoft 365 pro podnik, jako je Office 365 Enterprise E3 nebo Enterprise E5.
   > [!NOTE] 
   > Plány aplikací Microsoft 365 pro firmy a Microsoft 365 Business Premium neobsahují aplikace Microsoft 365 pro podnik.
- Musíte povolit [aktivaci sdíleného počítače](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Můžete také stáhnout a spustit [Pomocníka pro podporu a obnovení Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) pro systém Microsoft 365 v režimu aktivace sdíleného počítače.

Další informace o požadavcích, pokyny k instalaci a pokyny k vlastním instalacím pomocí nástroje pro nasazení Office najdete v článku [nasazení aplikací Microsoft 365 pro podnik pomocí služby Vzdálená plocha](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Oprava chyb souvisejících se aktivací sdíleného počítače:
- Přečtěte si článek [Poradce při potížích s aktivací sdílené počítače pro aplikace Microsoft 365 pro podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Přečtěte si téma zaměřené na [resetování stavu aktivace Microsoft 365 Apps pro podniky](https://go.microsoft.com/fwlink/?linkid=2109218).

Pokud chcete nainstalovat aplikace Microsoft 365 pro podnik v rámci služby RDS z centra pro správu Microsoft 365, ***které používá výchozí nastavení instalace***, postupujte takto:

1.    Zkontrolujte, jaké máte předplatné. [Zjistěte, jak](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    V případě potřeby přepněte na jiné předplatné. [Zjistěte, jak](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Pokud už máte Office nainstalovaný na serveru RDS pomocí jakéhokoliv jiného předplatného Microsoftu, odinstalujte ho. Například v **ovládacím panelu**  >  **Odinstalujte program**. Pokud máte problémy, odinstalujte ho pomocí nástroje [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) .
4.    Na serveru RDS se přihlaste do centra pro správu Microsoft 365 s účtem správce a [nainstalujte si aplikace Microsoft 365 pro podniky](https://portal.office.com/OLS/MySoftware.aspx).
5.    Po instalaci Office se ***Neotevírejte ani se přihlaste*** k žádným aplikacím Office.
6.    Na serveru RDS povolte aktivaci sdíleného počítače úpravou registru pomocí následujícího postupu:
   1. Klikněte pravým tlačítkem myši na tlačítko Windows v levém dolním rohu obrazovky a vyberte **Spustit**. Do pole Otevřít zadejte **Regedit**a pak vyberte **OK**.
   2. Když se zobrazí výzva, aby Editor registru mohl v zařízení dělat změny, vyberte **Ano** .
   3. V editoru registru přidejte hodnotu řetězce **SharedComputerLicensing** s nastavením 1 v části HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.
   4. Na serveru RDS se ***přihlaste jako koncový uživatel*** a [Ověřte, jestli je povolená aktivace sdíleného počítače pro Microsoft 365](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

