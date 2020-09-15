---
title: Odepřený přístup při prohlížení pracovního postupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688795"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="bbeb8-102">Odepřený přístup při prohlížení pracovního postupu</span><span class="sxs-lookup"><span data-stu-id="bbeb8-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="bbeb8-103">Pracovní postupy SharePoint 2013, které se pokoušíte odeslat e-mail skupině SharePoint, se můžou zdařit s chybovou zprávou "přístup odepřen", pokud členství ve skupině SharePointu není nastaveno na Everyone.</span><span class="sxs-lookup"><span data-stu-id="bbeb8-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="bbeb8-104">**Tento problém vyřešíte takto:**</span><span class="sxs-lookup"><span data-stu-id="bbeb8-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="bbeb8-105">Povolit všem zobrazit členy skupiny SharePointu</span><span class="sxs-lookup"><span data-stu-id="bbeb8-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="bbeb8-106">Odeberte skupinu SharePointu z řádku Komu nebo kopie e-mailu.</span><span class="sxs-lookup"><span data-stu-id="bbeb8-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="bbeb8-107">Pokud nechcete, aby byla viditelnost členství pro skupinu SharePointu změněna, přidejte uživatele do řádku Komu nebo kopie.</span><span class="sxs-lookup"><span data-stu-id="bbeb8-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="bbeb8-108">Pokud chcete zobrazit další podrobnosti, přečtěte si téma [http neautorizované na/_vti_bin/Client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="bbeb8-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  