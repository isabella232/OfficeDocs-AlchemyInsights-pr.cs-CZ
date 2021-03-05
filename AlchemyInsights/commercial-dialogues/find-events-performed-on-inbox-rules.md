---
title: Hledání událostí provedených u pravidel doručené pošty
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481275"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="cad55-102">Hledání událostí provedených u pravidel doručené pošty</span><span class="sxs-lookup"><span data-stu-id="cad55-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="cad55-103">Když pravidla doručené pošty vytváříte, měníte nebo odstraníte, zaznamenávají se události do protokolu auditování.</span><span class="sxs-lookup"><span data-stu-id="cad55-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="cad55-104">Tady je postup, jak je zkontrolovat:</span><span class="sxs-lookup"><span data-stu-id="cad55-104">Here's how to review them:</span></span>

1. <span data-ttu-id="cad55-105">Přejděte do Centra zabezpečení a dodržování předpisů [Office 365 & dodržování předpisů.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="cad55-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="cad55-106">Vyberte Hledat > v protokolu auditování.</span><span class="sxs-lookup"><span data-stu-id="cad55-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="cad55-107">Pokud vidíte oznámení, že je potřeba auditování zapnout, můžete ho teď zapnout.</span><span class="sxs-lookup"><span data-stu-id="cad55-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="cad55-108">Pokud tato funkce není zapnutá, výsledky hledání nebudou moct natahovat data z předchozích dat.</span><span class="sxs-lookup"><span data-stu-id="cad55-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="cad55-109">Vyberte pole Aktivity, najděte aktivity poštovní schránky Exchange a pak vyberte New-InboxRule vytvořit pravidlo doručené pošty z Outlook Web Appu.</span><span class="sxs-lookup"><span data-stu-id="cad55-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="cad55-110">Až budete hotovi, kliknutím mimo podokno podokno aktivit minimalizujte.</span><span class="sxs-lookup"><span data-stu-id="cad55-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="cad55-111">Zadejte rozsah dat a pak v poli Uživatelé vyberte uživatelské jméno uživatele, kterého chcete prozkoumat.</span><span class="sxs-lookup"><span data-stu-id="cad55-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="cad55-112">Můžete vybrat víc uživatelů najednou.</span><span class="sxs-lookup"><span data-stu-id="cad55-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="cad55-113">Vyberte Hledat.</span><span class="sxs-lookup"><span data-stu-id="cad55-113">Select Search.</span></span> <span data-ttu-id="cad55-114">Aktivity se zobrazí v části Výsledky.</span><span class="sxs-lookup"><span data-stu-id="cad55-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="cad55-115">Pokud chcete zobrazit podrobnosti, vyberte aktivitu a pak vyberte Další informace.</span><span class="sxs-lookup"><span data-stu-id="cad55-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="cad55-116">V části Parametry můžete vidět název pravidla, sadu podmínek a akce, které bude pravidlo provádět.</span><span class="sxs-lookup"><span data-stu-id="cad55-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="cad55-117">Další informace najdete v protokolu auditování Office 365, kde najdete řešení běžných scénářů.</span><span class="sxs-lookup"><span data-stu-id="cad55-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>