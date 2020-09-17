---
title: Nasazení Teams jako samostatné nebo pomocí nových nebo existujících instalací Office
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
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806752"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Nasazení Teams jako samostatné nebo pomocí nových nebo existujících instalací Office

Microsoft Teams je teď součástí ***nových instalací*** aplikací Microsoft 365 pro podniky, Microsoft 365 Apps pro firmy a Office for Mac. Další informace najdete v tématu [kdy se začnou aplikace Microsoft Teams zahrnout do nových instalací Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Kromě toho, že počínaje verzí 1906 v aktuálním kanálu budou týmy ***přidány do existujících instalací*** aplikací Microsoft 365 (a Microsoft 365 pro firmy) na zařízeních se systémem Windows při aktualizaci stávající instalace na nejnovější verzi. Další informace najdete v článku [o existujících instalacích Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Pokud nechcete čekat na tento plán zavedení, můžete pro uživatele nasadit týmy jako samostatné, a to podle [těchto pokynů](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   nebo můžete uživatelům, kteří si k sobě nainstalují týmy  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Pokud vaše organizace neumožňuje nasadit týmy, máme k dispozici kroky, které můžete využít k ***vyloučení týmů*** z [nových](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) nebo [existujících](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) instalací Office. Pokud chcete, aby se aplikace Teams instalovaly, ale nechcete, aby se týmy automaticky spouštěly po instalaci, přečtěte si téma [Zabránění spuštění Microsoft Teams po instalaci](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Pokud chcete ***odinstalovat týmy*** ze zařízení se systémem Windows, přečtěte si článek [odinstalace Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Chcete-li vyčistit Microsoft Teams z více cílových počítačů nebo uživatelů, přečtěte si téma [nasazení Microsoft Teams Cleanup](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Pokud používáte sdílené počítače, služby vzdálené plochy (RDS) nebo infrastrukturu virtuálních počítačů (VDI), podívejte se na téma [sdílený počítač a prostředí VDI v Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Pokud používáte Office pro Mac, přečtěte si článek [instalace Microsoft Teams na Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Po instalaci jsou týmy [automaticky aktualizovány](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) přibližně každé dva týdny pomocí nových funkcí a aktualizací kvality. 