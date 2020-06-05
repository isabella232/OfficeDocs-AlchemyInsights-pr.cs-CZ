---
title: Byl překročen denní limit e-mailu. Pracovní postup je pozastaven.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580326"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="00bab-103">Byl překročen denní limit e-mailu.</span><span class="sxs-lookup"><span data-stu-id="00bab-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="00bab-104">Pracovní postup je pozastaven.</span><span class="sxs-lookup"><span data-stu-id="00bab-104">Workflow is suspended.</span></span>

<span data-ttu-id="00bab-105">Tato chyba může být přijata v následujících scénářích:</span><span class="sxs-lookup"><span data-stu-id="00bab-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="00bab-106">V SharePointu Online máte pracovní postup, který používá typ platformy pracovního postupu SharePointu 2010 nebo SharePointu 2013.</span><span class="sxs-lookup"><span data-stu-id="00bab-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="00bab-107">Pracovní postup je nakonfigurován tak, aby odesílá vlastní e-mailovou zprávu více než 200 uživatelům najednou, více než 10 000 příjemcům denně nebo více než 30 zpráv za minutu.</span><span class="sxs-lookup"><span data-stu-id="00bab-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="00bab-108">Při spuštění pracovního postupu se e-mailová zpráva neodesílá a zjistíte následující chování:</span><span class="sxs-lookup"><span data-stu-id="00bab-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="00bab-109">U pracovního postupu s typem platformy SharePointu 2013 přejděte na stránku **Stav pracovního postupu.**</span><span class="sxs-lookup"><span data-stu-id="00bab-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="00bab-110">Na stránce Stav pracovního postupu je **vnitřní stav** nastaven na **počáteční**hodnotu a v bublině informace se zobrazí možnost **Nelze odeslat příjemci**.</span><span class="sxs-lookup"><span data-stu-id="00bab-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="00bab-111">Chcete-li tento problém vyřešit, nakonfigurujte pracovní postup tak, aby odesílal e-mailové zprávy bez překročení [limitů odesílatele Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="00bab-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="00bab-112">Můžete například použít pozastavení v pracovním postupu, odeslat e-mail skupině Microsoft 365, distribuční skupině nebo skupině zabezpečení s povolenou poštou nebo odeslat zprávu méně než 200 příjemcům najednou.</span><span class="sxs-lookup"><span data-stu-id="00bab-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="00bab-113">Další informace naleznete v následujícím [článku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="00bab-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="00bab-114">Související témata</span><span class="sxs-lookup"><span data-stu-id="00bab-114">Related topics</span></span>
- [<span data-ttu-id="00bab-115">Vytvořit tok</span><span class="sxs-lookup"><span data-stu-id="00bab-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="00bab-116">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="00bab-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 