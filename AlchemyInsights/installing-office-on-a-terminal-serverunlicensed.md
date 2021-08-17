---
title: Instalace office na terminálový server – nelicencovaná
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
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055151"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalace Office na terminálový server

Pro nasazení Microsoft 365 Apps pro velké organizace na Windows serveru pomocí Vzdálené plochy (RDS), dříve pojmenovaného Terminálová služba:
  
- Musíte mít předplatné Microsoft 365, které zahrnuje Microsoft 365 Apps pro velké organizace, jako je Office 365 Enterprise E3 nebo Enterprise E5. Plány Microsoft 365 Apps pro firmy a Microsoft 365 Apps pro firmy Premium plány nezahrnují Microsoft 365 Apps pro velké organizace.

- Musíte povolit aktivaci [sdíleného počítače](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Pokud chcete nainstalovat Microsoft 365 Apps pro velké organizace rds z Centrum pro správu Microsoftu 365, který používá výchozí nastavení ***instalace***, postupujte podle následujících kroků.

> [!TIP]
> Můžete si taky stáhnout a spustit [microsoftový Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) a nainstalovat Microsoft 365 Apps pro velké organizace v režimu aktivace sdíleného počítače.
  
1. Zkontrolujte, Microsoft 365 předplatné máte. [Zjistěte, jak na to](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. V případě potřeby přepněte na jiné Microsoft 365 předplatné. [Zjistěte, jak na to](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Pokud Office server RDS nainstalovaný pomocí jiných předplatných, Microsoft 365 odinstalovat. Například tak, že v Ovládacích panelech \> odinstalujete program. Pokud máte [problémy, Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) microsoftu odinstalovat.

4. Na serveru RDS se přihlaste k účtu Centrum pro správu Microsoftu 365 správce a [nainstalujte si Microsoft 365 Apps pro velké organizace](https://portal.office.com/OLS/MySoftware.aspx).

5. Po Office se ***neotev ít*** ani se k žádným aplikacím Office přihlásit.

6. Na serveru RDS povolte aktivaci sdíleného počítače úpravou registru takto:

1. Klikněte pravým tlačítkem na Windows v levém dolním rohu obrazovky a vyberte Spustit. Do pole Otevřít zadejte **regedit** a pak vyberte OK.

2. Po zobrazení výzvy k povolení editoru registru k provedení změn ve vašem zařízení vyberte Ano.

3. V Editoru registru přidejte řetězcovou hodnotu **SharedComputerLicensing** s nastavením 1 v části HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na serveru RDS se přihlaste jako koncový ***uživatel a*** ověřte, že je povolená aktivace sdíleného počítače [pro Microsoft 365 Apps pro velké organizace](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Další podrobnosti o předpokladech, pokyny k instalaci a pokyny k přizpůsobené instalaci pomocí nástroje pro nasazení Office najdete v tématu Nasazení Microsoft 365 Apps pro velké organizace pomocí služby [Vzdálená plocha](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Pokud chcete opravit chyby související s aktivací sdíleného počítače, přečtěte si prosím článek Řešení potíží s aktivací sdíleného počítače [pro Microsoft 365 Apps pro velké organizace](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  