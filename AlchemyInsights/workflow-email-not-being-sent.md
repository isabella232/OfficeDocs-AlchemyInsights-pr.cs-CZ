---
title: E-mail pracovního postupu se neposílá
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748982"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="14f31-102">E-mail pracovního postupu se neposílá pro seznam nebo knihovnu SharePointu</span><span class="sxs-lookup"><span data-stu-id="14f31-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="14f31-103">E-mail od pracovních postupů se neposílá všem uživatelům nebo jenom určitým uživatelům, nebo se zobrazí chyba **: e-mailovou zprávu nelze odeslat. Zkontrolujte, jestli má e-mail platného příjemce**.</span><span class="sxs-lookup"><span data-stu-id="14f31-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="14f31-104">Zkontrolujte, jestli uživatel existuje ve skupině oprávnění **všech lidí** (seznam informací o uživateli) pro tuto kolekci webů.</span><span class="sxs-lookup"><span data-stu-id="14f31-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="14f31-105">Ukázka přímé adresy URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="14f31-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="14f31-106">Pokud uživatel neexistuje, zkontrolujte, jestli je uživatel přihlášený na stránku.</span><span class="sxs-lookup"><span data-stu-id="14f31-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="14f31-107">Pokud je to externí uživatel, ujistěte se, že Pozvánka byla přijata.</span><span class="sxs-lookup"><span data-stu-id="14f31-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="14f31-108">Pokud uživatel ve skupině oprávnění existuje, zkontrolujte správnost e-mailové adresy.</span><span class="sxs-lookup"><span data-stu-id="14f31-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="14f31-109">Pokud tady není nastavená e-mailová adresa uživatele, vytvořte pro tohoto uživatele ukázkové upozornění, které vynutí synchronizaci tohoto uživatelského účtu z profilů uživatelů SharePointu do této kolekce webů.</span><span class="sxs-lookup"><span data-stu-id="14f31-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="14f31-110">E-maily od pracovních postupů se odesílají správcům kolekce webů, ale ne ostatním uživatelům a zobrazují se vám chybové zprávy **http <span>:</span>//URL/_vti_bin/Client.XVC.SP.Utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="14f31-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="14f31-111">[Pokud odešlete e-mail skupině SharePointu](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups), přečtěte si článek přístup odepřen.</span><span class="sxs-lookup"><span data-stu-id="14f31-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="14f31-112">Ověřte také, že funkce kolekce webů **režimu uzamčení oprávnění uživatelů s omezeným přístupem** není aktivní.</span><span class="sxs-lookup"><span data-stu-id="14f31-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="14f31-113">Související témata</span><span class="sxs-lookup"><span data-stu-id="14f31-113">Related topics</span></span>
<span data-ttu-id="14f31-114">Chcete vyzkoušet tok Microsoftu v SharePointu Online?</span><span class="sxs-lookup"><span data-stu-id="14f31-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="14f31-115">Vytvoření toku</span><span class="sxs-lookup"><span data-stu-id="14f31-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="14f31-116">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="14f31-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


