---
title: Nasazení Teams jako samostatného nebo s novými nebo stávajícími instalacemi Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617888"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Nasazení Teams jako samostatného nebo s novými nebo stávajícími instalacemi Office

Microsoft Teams je teď součástí nových instalací Aplikací Microsoft 365 pro ***podniky,*** Aplikací Microsoft 365 pro firmy a Office for Mac. Další informace najdete v [tématu Kdy se microsoft teams začnou zadát do nových instalací Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Kromě toho počínaje verzí 1906 v aktuálním kanálu budou teams ***přidány do stávajících instalací*** aplikací Microsoft 365 Apps pro podniky (a Aplikací Microsoft 365 pro firmy) na zařízeních se systémem Windows při aktualizaci stávající instalace na nejnovější verzi. Další informace najdete v [tématu A co stávající instalace Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Pokud nechcete čekat na tento plán zavádění, můžete nasadit Teams jako samostatné pro uživatele [podle těchto pokynů](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)nebo můžete nechat uživatele nainstalovat Teams pro sebe z    [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Pokud vaše organizace není připravená k nasazení Teams, máme kroky, které můžete udělat, abyste ***vyřadili Teams*** z [nových](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) nebo [stávajících](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) instalací Office. Pokud chcete, aby se Teams nainstalovaly, ale nechcete, aby se Teams po instalaci automaticky spouštěl, přečtěte si [přečtěte si přečtěte si, jak zabránit automatickému spuštění Microsoft Teams po instalaci](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Informace o ***odinstalaci Teams*** ze zařízení se systémem Windows najdete v [tématu Odinstalace Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Informace o vyčištění aplikace Microsoft Teams od více cílových počítačů nebo uživatelů naleznete v [tématu Vyčištění nasazení v Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Pokud používáte sdílené počítače, službu Vzdálená plocha (RDS) nebo infrastrukturu virtuálních ploch (VDI), přečtěte si [tématu Sdílený počítač a prostředí VDI v Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Pokud používáte Office for Mac, přečtěte si informace o [instalacích Microsoft Teams na Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Po instalaci teams se [automaticky aktualizuje](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) přibližně každé dva týdny s novými funkcemi a aktualizacemi kvality. 