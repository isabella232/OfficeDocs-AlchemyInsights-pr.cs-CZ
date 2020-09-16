---
title: Odložit upgrade na Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741764"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="c1cd5-102">Odložení upgradu týmu řízeného společností Microsoft</span><span class="sxs-lookup"><span data-stu-id="c1cd5-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="c1cd5-103">**Důležité**: Tento problém můžeme pomoct vyřešit pomocí diagnostické podpory, ale vypadá to, že nepoužíváte nové centrum pro správu.</span><span class="sxs-lookup"><span data-stu-id="c1cd5-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="c1cd5-104">Pokud chcete nové centrum pro správu použít, posuňte přepínač v pravém horním rohu, který říká **nové centrum pro správu** vpravo.</span><span class="sxs-lookup"><span data-stu-id="c1cd5-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="c1cd5-105">V novém centru pro správu klikněte na widget " **Potřebuji nápovědu?** ", zadejte "odložit upgrade týmů" a spusťte diagnostický nástroj podle pokynů.</span><span class="sxs-lookup"><span data-stu-id="c1cd5-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="c1cd5-106">Pokud jste obdrželi sdělení o automatizovaném upgradu založeném na Microsoftu ze Skypu pro firmy do Microsoft teams a chcete automatické upgrade odložit na pozdější datum, může se Váš globální správce přihlásit na portál pro [správu portálu](https://admin.teams.microsoft.com/dashboard) a po výběru tlačítka pro **stav aktualizace** v části Microsoft Teams upgrade vyberte tlačítko **odložit** .</span><span class="sxs-lookup"><span data-stu-id="c1cd5-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="c1cd5-107">Pokud chcete zobrazit nové datum automatizovaného upgradu vašeho klienta na Microsoft teams, aktualizujte stránku portálu pro správu Teams.</span><span class="sxs-lookup"><span data-stu-id="c1cd5-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="c1cd5-108">**Poznámka:** Tlačítko **odložení** bude k dispozici pouze v případě, že jste dostali oznámení centra zpráv s cílem automatického upgradu.</span><span class="sxs-lookup"><span data-stu-id="c1cd5-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="c1cd5-109">Globální správci můžou pomocí [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) získat další informace o aktuálním stavu upgradu.</span><span class="sxs-lookup"><span data-stu-id="c1cd5-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
