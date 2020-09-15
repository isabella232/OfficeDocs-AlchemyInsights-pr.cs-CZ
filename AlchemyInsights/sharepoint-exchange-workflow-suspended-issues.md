---
title: Začínáme se SharePointem Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700700"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="49e10-102">Pracovní postupy v SharePointu</span><span class="sxs-lookup"><span data-stu-id="49e10-102">Workflows in SharePoint</span></span>

<span data-ttu-id="49e10-103">Pokud pracovní postupy SharePointu neodesílají e-maily, mohla by vaše organizace vyznamenala limity pro odesílatele Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="49e10-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="49e10-104">Chybová zpráva "pracovní postup je pozastaven" se může zobrazit, pokud máte některou z následujících věcí:</span><span class="sxs-lookup"><span data-stu-id="49e10-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="49e10-105">V SharePointu Online máte pracovní postup používající typ platformy SharePoint 2010 nebo SharePoint 2013 pracovního postupu.</span><span class="sxs-lookup"><span data-stu-id="49e10-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="49e10-106">Pracovní postup je nakonfigurovaný tak, aby posílal vlastní e-mailovou zprávu více než 200 uživatelům najednou, více než 10 000 příjemců za den nebo více než 30 zpráv za minutu.</span><span class="sxs-lookup"><span data-stu-id="49e10-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="49e10-107">Když spustíte pracovní postup, e-mailová zpráva není odeslaná a zobrazí se chybová zpráva, vnitřní stav je nastaven na pozastaveno nebo se nedaří Odeslat příjemci.</span><span class="sxs-lookup"><span data-stu-id="49e10-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="49e10-108">Další informace najdete v následujícím [článku](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="49e10-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

