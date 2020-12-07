---
title: Co dělat, když funkce Azure v Microsoft Edge nefungují správně
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583308"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="73eba-102">Co dělat, když funkce Azure v Microsoft Edge nefungují správně</span><span class="sxs-lookup"><span data-stu-id="73eba-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="73eba-103">Microsoft Edge má [známé problémy](https://go.microsoft.com/fwlink/?linkid=2140608) související se zónami zabezpečení a může mít vliv na to, jak se uživatelé Azure přihlašují do centra pro správu Windows.</span><span class="sxs-lookup"><span data-stu-id="73eba-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="73eba-104">Pokud máte v Microsoft Edge potíže s používáním funkcí Azure, vyzkoušejte následující postup:</span><span class="sxs-lookup"><span data-stu-id="73eba-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="73eba-105">V nabídce **Start** vyhledejte **Možnosti Internetu** a vyberte je.</span><span class="sxs-lookup"><span data-stu-id="73eba-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="73eba-106">V dialogovém okně **Internet – vlastnosti** přejděte na kartu **zabezpečení** .</span><span class="sxs-lookup"><span data-stu-id="73eba-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="73eba-107">Vyberte zónu **Důvěryhodné servery** a pak klikněte na tlačítko **weby** .</span><span class="sxs-lookup"><span data-stu-id="73eba-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="73eba-108">V dialogovém okně **Důvěryhodné servery** zadejte adresu URL brány [https://login.microsoftonline.com](https://login.microsoftonline.com) a taky a [https://login.live.com](https://login.live.com) pak vyberte **Zavřít**.</span><span class="sxs-lookup"><span data-stu-id="73eba-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="73eba-109">V dialogovém okně **Internet – vlastnosti** přejděte na kartu **soukromí** .</span><span class="sxs-lookup"><span data-stu-id="73eba-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="73eba-110">V části **blokování automaticky otevíraných oken** vyberte **Nastavení**.</span><span class="sxs-lookup"><span data-stu-id="73eba-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="73eba-111">V dialogovém okně, které se otevře, přidejte adresu URL brány a taky [https://login.microsoftonline.com](https://login.microsoftonline.com) a [https://login.live.com](https://login.live.com) pak vyberte **Zavřít**.</span><span class="sxs-lookup"><span data-stu-id="73eba-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
