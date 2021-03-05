---
title: Zjistěte, kdo nastaví přeposílání v poštovní schránce a jak
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481203"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="45957-102">Zjistěte, kdo nastaví přeposílání v poštovní schránce a jak</span><span class="sxs-lookup"><span data-stu-id="45957-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="45957-103">Pokud bylo u poštovní schránky nastavené externí přeposílání, aktivita se audituje jako součást rutiny Set-Mailbox Serveru.</span><span class="sxs-lookup"><span data-stu-id="45957-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="45957-104">Tady je postup, jak najít aktivitu v protokolu auditování:</span><span class="sxs-lookup"><span data-stu-id="45957-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="45957-105">Přejděte do Centra zabezpečení a dodržování předpisů [Office 365 & dodržování předpisů.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="45957-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="45957-106">Vyberte **Hledat v** protokolu >  **auditování.**</span><span class="sxs-lookup"><span data-stu-id="45957-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="45957-107">Pokud vidíte oznámení, že je potřeba auditování zapnout, můžete ho teď zapnout.</span><span class="sxs-lookup"><span data-stu-id="45957-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="45957-108">Pokud tato funkce není zapnutá, výsledky hledání nebudou moct natahovat data z předchozích dat.</span><span class="sxs-lookup"><span data-stu-id="45957-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="45957-109">Ujistěte **se, že** je v poli Aktivity nastavené zobrazení **výsledků pro všechny aktivity** (výchozí nastavení).</span><span class="sxs-lookup"><span data-stu-id="45957-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="45957-110">Zadejte rozsah dat.</span><span class="sxs-lookup"><span data-stu-id="45957-110">Specify the date range.</span></span> <span data-ttu-id="45957-111">Nemusíte zazadat uživatelské jméno.</span><span class="sxs-lookup"><span data-stu-id="45957-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="45957-112">Vyberte **Hledat.**</span><span class="sxs-lookup"><span data-stu-id="45957-112">Select **Search**.</span></span> <span data-ttu-id="45957-113">Aktivity se zobrazí v části **Výsledky.**</span><span class="sxs-lookup"><span data-stu-id="45957-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="45957-114">Vyberte **Výsledky filtru a** potom do  pole Filtru aktivity zadejte Nastavit poštovní schránku. </span><span class="sxs-lookup"><span data-stu-id="45957-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="45957-115">Vrátí všechny **aktivity nastavené poštovní schránky.**</span><span class="sxs-lookup"><span data-stu-id="45957-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="45957-116">Pokud chcete zobrazit podrobnosti, vyberte aktivitu a pak **vyberte Další informace.**</span><span class="sxs-lookup"><span data-stu-id="45957-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="45957-117">V **části Parametry** můžete vidět e-mailovou adresu pro přeposílání nastavenou v poštovní schránce.</span><span class="sxs-lookup"><span data-stu-id="45957-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="45957-118">ID **uživatele** představuje uživatele, který u poštovní schránky nastavil externí přeposílání.</span><span class="sxs-lookup"><span data-stu-id="45957-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="45957-119">Další informace najdete v protokolu [auditování Office 365,](https://go.microsoft.com/fwlink/?linkid=2103944)kde najdete řešení běžných scénářů.</span><span class="sxs-lookup"><span data-stu-id="45957-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>