---
title: Čtení protokolů auditování u odstraněných událostí
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429374"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="0b9a3-102">Čtení protokolů auditování u odstraněných událostí</span><span class="sxs-lookup"><span data-stu-id="0b9a3-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="0b9a3-103">Tady je postup:</span><span class="sxs-lookup"><span data-stu-id="0b9a3-103">Here's how to do this:</span></span>

1. <span data-ttu-id="0b9a3-104">Přejděte do Centra zabezpečení a dodržování předpisů [Office 365 & dodržování předpisů.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="0b9a3-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="0b9a3-105">Vyberte **Hledat**  >  [**v protokolu auditování.**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="0b9a3-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="0b9a3-106">Pokud vidíte oznámení, že je potřeba tuto funkci zapnout, můžete ji teď zapnout.</span><span class="sxs-lookup"><span data-stu-id="0b9a3-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="0b9a3-107">Pokud tato funkce není zapnutá, výsledky hledání nebudou moct natahovat data z předchozích dat.</span><span class="sxs-lookup"><span data-stu-id="0b9a3-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="0b9a3-108">Vyberte **Aktivity a** pak vyhledejte aktivity poštovní schránky systému **Exchange.**</span><span class="sxs-lookup"><span data-stu-id="0b9a3-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="0b9a3-109">Vyberte **odstraněné zprávy ze složky Odstraněná** pošta a Přesunuté zprávy do **složky Odstraněná** pošta.</span><span class="sxs-lookup"><span data-stu-id="0b9a3-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="0b9a3-110">Až budete hotovi, kliknutím mimo podokno  podokno aktivit minimalizujte.</span><span class="sxs-lookup"><span data-stu-id="0b9a3-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="0b9a3-111">Zadejte rozsah dat a v  poli Uživatelé vyberte uživatelské jméno uživatele, kterého chcete prozkoumat.</span><span class="sxs-lookup"><span data-stu-id="0b9a3-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="0b9a3-112">Můžete vybrat víc uživatelů najednou.</span><span class="sxs-lookup"><span data-stu-id="0b9a3-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="0b9a3-113">Vyberte **Hledat.**</span><span class="sxs-lookup"><span data-stu-id="0b9a3-113">Select **Search**.</span></span> <span data-ttu-id="0b9a3-114">Aktivity se zobrazí v části **Výsledky.**</span><span class="sxs-lookup"><span data-stu-id="0b9a3-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="0b9a3-115">Pokud chcete zobrazit podrobnosti, vyberte aktivitu a pak **vyberte Další informace.**</span><span class="sxs-lookup"><span data-stu-id="0b9a3-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="0b9a3-116">V poli **AffectedItems** se zobrazí další informace o odstraněné položce, například řádek předmětu a umístění položky při odstranění.</span><span class="sxs-lookup"><span data-stu-id="0b9a3-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="0b9a3-117">Odstraněné položky nelze obnovit pomocí funkce protokolu auditování.</span><span class="sxs-lookup"><span data-stu-id="0b9a3-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="0b9a3-118">Pokud chcete obnovit odstraněné položky, podívejte se na část Obnovení odstraněných položek nebo e-mailů [v Outlook Web Appu.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="0b9a3-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="0b9a3-119">Další informace najdete v protokolu [auditování Office 365,](https://go.microsoft.com/fwlink/?linkid=2103944)kde najdete řešení běžných scénářů.</span><span class="sxs-lookup"><span data-stu-id="0b9a3-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
