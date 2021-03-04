---
title: Vyhledání IP adresy v protokolu auditování
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429363"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="ac7b1-102">Vyhledání IP adresy v protokolu auditování</span><span class="sxs-lookup"><span data-stu-id="ac7b1-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="ac7b1-103">IP adresa odpovídající aktivitě provedené uživatelem nebo správcem se zobrazuje v protokolech auditování.</span><span class="sxs-lookup"><span data-stu-id="ac7b1-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="ac7b1-104">Protokolované jsou taky informace o klientovi.</span><span class="sxs-lookup"><span data-stu-id="ac7b1-104">The client information is also logged.</span></span> <span data-ttu-id="ac7b1-105">Tady je postup, jak identifikovat IP adresu:</span><span class="sxs-lookup"><span data-stu-id="ac7b1-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="ac7b1-106">Přejděte do Centra zabezpečení a dodržování předpisů [Office 365 & dodržování předpisů.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="ac7b1-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="ac7b1-107">Vyberte **Hledat**  >  **[v protokolu auditování.](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="ac7b1-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="ac7b1-108">Pokud uvidíte oznámení, že je potřeba auditování zapnout, můžete ho teď zapnout.</span><span class="sxs-lookup"><span data-stu-id="ac7b1-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="ac7b1-109">Pokud tato funkce není povolená, výsledky hledání nebudou moct natahovat data z předchozích dat.</span><span class="sxs-lookup"><span data-stu-id="ac7b1-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="ac7b1-110">Pokud vás zajímá určitá aktivita, vyberte ji v **seznamu** aktivity. v opačném případě se pro vybraného uživatele vrátí všechny aktivity.</span><span class="sxs-lookup"><span data-stu-id="ac7b1-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="ac7b1-111">Upozorňujeme, že některé aktivity nemusí být dostupné pro výběr z **nabídky** Aktivity. Pokud ale vyberete zobrazit  výsledky pro všechny aktivity (výchozí nastavení), vrátí se tyto položky auditování.</span><span class="sxs-lookup"><span data-stu-id="ac7b1-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="ac7b1-112">Zadejte rozsah dat a  v poli Uživatelé vyberte uživatelské jméno uživatele, kterého chcete prozkoumat.</span><span class="sxs-lookup"><span data-stu-id="ac7b1-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="ac7b1-113">Vyberte **Hledat.**</span><span class="sxs-lookup"><span data-stu-id="ac7b1-113">Select **Search**.</span></span> <span data-ttu-id="ac7b1-114">Aktivity se zobrazí v části **Výsledky.**</span><span class="sxs-lookup"><span data-stu-id="ac7b1-114">The activities appear under **Results**.</span></span> <span data-ttu-id="ac7b1-115">Pro každou aktivitu se můžete podívat na IP adresu.</span><span class="sxs-lookup"><span data-stu-id="ac7b1-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="ac7b1-116">Pokud chcete zobrazit podrobnosti, vyberte aktivitu a pak **vyberte Další informace.**</span><span class="sxs-lookup"><span data-stu-id="ac7b1-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="ac7b1-117">Další informace najdete v protokolu [auditování Office 365,](https://go.microsoft.com/fwlink/?linkid=2103944)kde najdete řešení běžných scénářů.</span><span class="sxs-lookup"><span data-stu-id="ac7b1-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>