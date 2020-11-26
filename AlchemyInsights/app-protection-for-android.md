---
title: Nastavení zásad ochrany aplikací pro Android v Microsoft Intune
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003997"
- "7057"
ms.openlocfilehash: 327df6e0a901037cd929cb845f805466d9bd4eff
ms.sourcegitcommit: 81c86027933c06db08d264918f2698d9c9a1659a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/20/2020
ms.locfileid: "49447293"
---
# <a name="android-app-protection-policy-settings-in-microsoft-intune"></a><span data-ttu-id="743cc-102">Nastavení zásad ochrany aplikací pro Android v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="743cc-102">Android app protection policy settings in Microsoft Intune</span></span>

<span data-ttu-id="743cc-103">Existují tři kategorie nastavení zásad ochrany aplikací pro zařízení s Androidem:</span><span class="sxs-lookup"><span data-stu-id="743cc-103">There are three categories of app protection policy settings for Android devices:</span></span>

<span data-ttu-id="743cc-104">**Ochrana dat** určuje způsob, jakým se zpracovávají data společnosti, například jestli jde data zkopírovat nebo vložit do jiné aplikace nebo jestli se dá snímek obrazovky považovat za aplikaci.</span><span class="sxs-lookup"><span data-stu-id="743cc-104">**Data protection** controls how company data is handled, such as, whether data can be copied or pasted to a different app or whether a screenshot can be taken of the app.</span></span> <span data-ttu-id="743cc-105">Nastavení taky vynucuje šifrování v podnikových datech a řídí, jestli se některá data můžou synchronizovat s aplikacemi nativního zařízení, jako je seznam kontaktů nebo webový prohlížeč.</span><span class="sxs-lookup"><span data-stu-id="743cc-105">The settings also enforce encryption on company data and manage whether certain data can be synced with the native device apps, like the contact list or web browser.</span></span> <span data-ttu-id="743cc-106">Další informace najdete v tématu [Ochrana dat](https://go.microsoft.com/fwlink/?linkid=2135259).</span><span class="sxs-lookup"><span data-stu-id="743cc-106">To learn more, see [Data protection](https://go.microsoft.com/fwlink/?linkid=2135259).</span></span>

<span data-ttu-id="743cc-107">**Požadavky na přístup** popisují, jak můžou uživatelé získat přístup k aplikaci.</span><span class="sxs-lookup"><span data-stu-id="743cc-107">**Access requirements** guides how users can access an app.</span></span> <span data-ttu-id="743cc-108">Aplikace může například vyžadovat, aby zadal pro přístup k tomuto kódu PIN nebo otisk prstu.</span><span class="sxs-lookup"><span data-stu-id="743cc-108">For example, an app could require the user to enter a PIN or fingerprint to access it.</span></span> <span data-ttu-id="743cc-109">Další informace najdete v článku [požadavky na přístup](https://go.microsoft.com/fwlink/?linkid=2135260).</span><span class="sxs-lookup"><span data-stu-id="743cc-109">To learn more, see [Access requirements](https://go.microsoft.com/fwlink/?linkid=2135260).</span></span>

<span data-ttu-id="743cc-110">**Podmínkou spuštění** se řídí nastavení zabezpečení pro aplikaci, jako je třeba maximální počet pokusů o připnutí před uzamčením nebo minimální operační systém potřebný ke spuštění aplikace.</span><span class="sxs-lookup"><span data-stu-id="743cc-110">**Conditional launch** governs the sign-in security settings for an app, such as, the maximum PIN attempts before lockout or the minimum operating system needed to run the app.</span></span> <span data-ttu-id="743cc-111">Další informace najdete v tématu [podmíněné spuštění](https://go.microsoft.com/fwlink/?linkid=2135507).</span><span class="sxs-lookup"><span data-stu-id="743cc-111">To learn more, see [Conditional launch](https://go.microsoft.com/fwlink/?linkid=2135507).</span></span>
