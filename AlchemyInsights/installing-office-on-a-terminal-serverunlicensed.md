---
title: Instalace Office na terminálový server – nelicencovaná
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663110"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalace Office na terminálový server

Pro nasazení aplikací Microsoft 365 pro podnik na Windows serveru pomocí vzdálené plochy (RDS), dřív s názvem Terminálová služba:
  
- Musíte mít předplatné Microsoft 365, které obsahuje aplikace Microsoft 365 pro podniky, jako je třeba Office 365 Enterprise E3 nebo Enterprise E5. Plány aplikací Microsoft 365 pro firmy a Microsoft 365 Apps for Business Premium neobsahují aplikace Microsoft 365 pro firmy.

- Je třeba povolit [aktivaci sdílené počítače](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Pokud chcete nainstalovat aplikace Microsoft 365 pro podnik v rámci služby RDS z centra pro správu Microsoft 365, ***které používá výchozí nastavení instalace***, postupujte takto:

> [!TIP]
> Můžete také stáhnout a spustit [Pomocníka pro podporu a obnovení Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) pro systém Microsoft 365 v režimu aktivace sdíleného počítače.
  
1. Podívejte se na předplatné Microsoft 365. [Zjistěte, jak](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. V případě potřeby přejděte na jiné předplatné Microsoft 365. [Zjistěte, jak](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Pokud už máte Office nainstalovaný na serveru RDS pomocí jakéhokoli jiného předplatného Microsoft 365, odinstalujte ho. Například v ovládacím panelu \> Odinstalujte program. Pokud máte problémy, odinstalujte ho pomocí nástroje [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) .

4. Na serveru RDS se přihlaste do centra pro správu Microsoft 365 s účtem správce a [nainstalujte si aplikace Microsoft 365 pro podniky](https://portal.office.com/OLS/MySoftware.aspx).

5. Po instalaci Office se ***Neotevírejte ani se přihlaste*** k žádným aplikacím Office.

6. Na serveru RDS povolte aktivaci sdíleného počítače úpravou registru pomocí následujícího postupu:

1. Klikněte pravým tlačítkem myši na tlačítko Windows v levém dolním rohu obrazovky a vyberte spustit. Do pole Otevřít zadejte **Regedit**a pak vyberte OK.

2. Když se zobrazí výzva, aby Editor registru mohl v zařízení dělat změny, vyberte Ano.

3. V editoru registru přidejte hodnotu řetězce **SharedComputerLicensing** s nastavením 1 v části HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.

7. Na serveru RDS se ***přihlaste jako koncový uživatel*** a [Ověřte, jestli je povolená aktivace sdíleného počítače pro Microsoft 365](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Další informace o požadavcích, pokyny k instalaci a pokyny k přizpůsobení instalací pomocí nástroje pro nasazení Office najdete v článku [nasazení aplikací Microsoft 365 pro podnik pomocí služby Vzdálená plocha](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Pokud chcete opravit chyby související s aktivací sdíleného počítače, přečtěte si článek [Poradce při potížích s aktivací sdílené počítače pro aplikace Microsoft 365 pro podnik](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  