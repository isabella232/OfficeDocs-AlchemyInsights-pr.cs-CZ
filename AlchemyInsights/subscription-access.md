---
title: Přístup k předplatnému
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807224"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="767d9-102">Nejde se přihlásit do Azure kvůli problémům s prohlížečem (prohlížeč se zablokuje, nenačte se atd.).</span><span class="sxs-lookup"><span data-stu-id="767d9-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="767d9-103">Pravděpodobně bude ovlivněn výpadek.</span><span class="sxs-lookup"><span data-stu-id="767d9-103">You might be impacted by an outage.</span></span> <span data-ttu-id="767d9-104">Zkontrolujte, jestli se nejedná o probíhající výpadek: [stav Azure](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="767d9-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="767d9-105">Odhlaste se ze všech aktivních relací Azure.</span><span class="sxs-lookup"><span data-stu-id="767d9-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="767d9-106">Začněte v soukromém nebo prohlížečinové režimu webového prohlížeče.</span><span class="sxs-lookup"><span data-stu-id="767d9-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="767d9-107">Můžete se taky pokusit aktualizovat prohlížeč, použít jiný prohlížeč, odstranit soubory cookie mezipaměti, pokud dřív nefunguje.</span><span class="sxs-lookup"><span data-stu-id="767d9-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="767d9-108">Další informace: [řešení potíží s přihlašováním](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="767d9-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="767d9-109">**Nelze získat přístup k předplatným**</span><span class="sxs-lookup"><span data-stu-id="767d9-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="767d9-110">Na [portálu Azure](https://portal.azure.com/)se ujistěte, že je v pravém horním rohu vybraná správná složka Azure.</span><span class="sxs-lookup"><span data-stu-id="767d9-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="767d9-111">V [centru účtů Azure](https://account.windowsazure.com/Subscriptions)zkontrolujte, jestli je použitý účet správcem účtu.</span><span class="sxs-lookup"><span data-stu-id="767d9-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="767d9-112">Další informace: [řešení potíží s žádným předplatným](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="767d9-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="767d9-113">**Nelze získat přístup k historii fakturace**</span><span class="sxs-lookup"><span data-stu-id="767d9-113">**Unable to access billing history**</span></span>

<span data-ttu-id="767d9-114">Správce účtu musí zajistit, aby uživatel, který přistupuje k fakturačním informacím, přidal do služby Azure Active Directory jako hosta uživatele: [Přidání nebo odstranění nového uživatele](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="767d9-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="767d9-115">Uživatel pak musí mít roli globálního správce: [přiřazení role uživatelům](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="767d9-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="767d9-116">Publikovat: uživateli je možné udělit fakturační přístup pomocí zásad RBAC: [udělte přístup k fakturaci](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="767d9-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="767d9-117">**Doporučené dokumenty**</span><span class="sxs-lookup"><span data-stu-id="767d9-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="767d9-118">Nemůžu se přihlásit ke správě svého předplatného Azure</span><span class="sxs-lookup"><span data-stu-id="767d9-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)