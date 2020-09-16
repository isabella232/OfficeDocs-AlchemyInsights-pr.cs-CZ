---
title: Byl překročen denní limit pro e-mail. Pracovní postup je pozastaven.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731556"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="2aa24-103">Byl překročen denní limit pro e-mail.</span><span class="sxs-lookup"><span data-stu-id="2aa24-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="2aa24-104">Pracovní postup je pozastaven.</span><span class="sxs-lookup"><span data-stu-id="2aa24-104">Workflow is suspended.</span></span>

<span data-ttu-id="2aa24-105">Tato chyba se zobrazí v následujících situacích:</span><span class="sxs-lookup"><span data-stu-id="2aa24-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="2aa24-106">V SharePointu Online máte pracovní postup používající typ platformy SharePoint 2010 nebo SharePoint 2013 pracovního postupu.</span><span class="sxs-lookup"><span data-stu-id="2aa24-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="2aa24-107">Pracovní postup je nakonfigurovaný tak, aby posílal vlastní e-mailovou zprávu více než 200 uživatelům najednou, více než 10 000 příjemců za den nebo více než 30 zpráv za minutu.</span><span class="sxs-lookup"><span data-stu-id="2aa24-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="2aa24-108">Po spuštění pracovního postupu se e-mailová zpráva neodešle a všimnete si následujícího chování:</span><span class="sxs-lookup"><span data-stu-id="2aa24-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="2aa24-109">U pracovního postupu s typem platformy SharePoint 2013 přejděte na stránku **stav pracovního postupu** .</span><span class="sxs-lookup"><span data-stu-id="2aa24-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="2aa24-110">Na stránce Stav pracovního **postupu je nastaven stav** **aktivní na zahájeno**a informační bublina **nemůže odeslat příjemci**.</span><span class="sxs-lookup"><span data-stu-id="2aa24-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="2aa24-111">Pokud chcete tento problém vyřešit, nakonfigurujte pracovní postup tak, aby odesílal e-mailové zprávy bez překročení [limitů odesílatelů Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="2aa24-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="2aa24-112">Můžete například použít příkaz pozastavit v pracovním postupu, odeslat e-mail skupině Microsoft 365, skupině zabezpečení s povoleným e-mailem nebo zaslat zprávu na méně než 200 příjemců najednou.</span><span class="sxs-lookup"><span data-stu-id="2aa24-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="2aa24-113">Další informace najdete v následujícím [článku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="2aa24-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="2aa24-114">Související témata</span><span class="sxs-lookup"><span data-stu-id="2aa24-114">Related topics</span></span>
- [<span data-ttu-id="2aa24-115">Vytvoření toku</span><span class="sxs-lookup"><span data-stu-id="2aa24-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="2aa24-116">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="2aa24-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 