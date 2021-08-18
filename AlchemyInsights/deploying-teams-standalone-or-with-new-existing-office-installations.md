---
title: Nasazení Teams jako samostatné nebo s novými nebo stávajícími Office instalacemi
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320115"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Nasazení Teams jako samostatné nebo s novými nebo stávajícími Office instalacemi

Microsoft Teams je teď součástí nových  instalací Microsoft 365 Apps pro velké organizace, Microsoft 365 Apps pro firmy a Office pro Mac. Další informace najdete v článku Kdy se Microsoft Teams do nových instalací [Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Od verze 1906 v aktuálním kanálu se Teams  přidá do stávajících instalací Microsoft 365 Apps pro velké organizace (a Microsoft 365 Apps pro firmy) na zařízeních s Windows, když aktualizujete stávající instalaci na nejnovější verzi. Další informace najdete v tématu [Co se stávajícími instalacemi Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Poznámka:** Pokud nechcete čekat na tento plán zavedení, můžete nasadit Teams jako samostatný [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) pro uživatele podle těchto pokynů nebo můžete nastavit, aby si uživatelé Teams sami pro sebe [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) z .

Pokud vaše organizace není připravená nasadit Teams, máme postup, jak vyloučit Teams z [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) nových [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) nebo stávajících instalací Office.  Pokud chcete Teams nainstalovat, ale nechcete, aby se Teams pro uživatele po instalaci automaticky s spouštěním, podívejte se na informace v tématu Zabránění automatickému spuštění Microsoft Teams po [instalaci](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Informace ***o odinstalaci Teams*** ze zařízení se spuštěnou Windows najdete v tématu [Odinstalace Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Informace o Microsoft Teams cílových počítačů nebo uživatelů najdete v tématu [Microsoft Teams nasazení](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Pokud používáte sdílené počítače, vzdálenou plochu (RDS) nebo Infrastruktura virtuálních klientských počítačů (VDI), podívejte se na informace v tématu Sdílené počítače a [prostředí VDI](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)s Microsoft Teams .

Pokud používáte Office pro Mac, Microsoft Teams na [Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Poznámka:** Po Teams se automaticky aktualizuje [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) přibližně každé dva týdny novými funkcemi a aktualizacemi kvality. 