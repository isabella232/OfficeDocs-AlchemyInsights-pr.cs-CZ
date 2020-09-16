---
title: Problémy s výkonem – SharePoint nebo OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771237"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="93a9b-102">SharePoint nebo OneDrive pomalý, nedostupný nebo nedostupný pro víc uživatelů</span><span class="sxs-lookup"><span data-stu-id="93a9b-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="93a9b-103">Pokud není SharePointový web dostupný pro víc uživatelů, kteří mají přístup dřív, může se jednat o dočasný problém služby.</span><span class="sxs-lookup"><span data-stu-id="93a9b-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="93a9b-104">[Zkontrolujte řídicí panel stavu služeb](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="93a9b-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="93a9b-105">**Přidání a licence uživatele**</span><span class="sxs-lookup"><span data-stu-id="93a9b-105">**Add and license the user**</span></span>

<span data-ttu-id="93a9b-106">Zkontrolujte, že [přiřadíte licence uživatelům v Microsoft 365 pro firmy](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="93a9b-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="93a9b-107">**Přiřazení oprávnění**</span><span class="sxs-lookup"><span data-stu-id="93a9b-107">**Assign Permissions**</span></span>

<span data-ttu-id="93a9b-108">Pokud má uživatel přiřazenou licenci na SharePointu a pořád obdrží zprávu o odepření přístupu, ujistěte se, že mají přiřazenou [příslušnou úroveň oprávnění](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="93a9b-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="93a9b-109">**Zvažte použití funkce žádost o přístup.**</span><span class="sxs-lookup"><span data-stu-id="93a9b-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="93a9b-110">[Funkce žádosti o přístup](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umožňuje lidem požádat o přístup k obsahu, na který teď nemají oprávnění k zobrazení.</span><span class="sxs-lookup"><span data-stu-id="93a9b-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="93a9b-111">**Povolit vlastní skript může způsobit problémy s odepřením přístupu**</span><span class="sxs-lookup"><span data-stu-id="93a9b-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="93a9b-112">Je jisté, že funkce *Povolit vlastní skript* může představovat odepřený přístup.</span><span class="sxs-lookup"><span data-stu-id="93a9b-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="93a9b-113">Seznam ovlivněných funkcí, důležité informace o zabezpečení a možnosti zakázání funkce.</span><span class="sxs-lookup"><span data-stu-id="93a9b-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="93a9b-114">Navštivte stránku [Povolit nebo zakázat vlastní skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="93a9b-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

