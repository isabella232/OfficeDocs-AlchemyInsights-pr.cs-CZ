---
title: Role správy privilegované identity
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088570"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="10998-102">Role správce privilegované identity</span><span class="sxs-lookup"><span data-stu-id="10998-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="10998-103">**Po aktivaci role nejsou udělována oprávnění**</span><span class="sxs-lookup"><span data-stu-id="10998-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="10998-104">Když aktivujete roli ve správě privilegované identity služby Azure AD (PIM), nemusí se aktivace okamžitě šířit na všechny portály, které vyžadují privilegovanou roli.</span><span class="sxs-lookup"><span data-stu-id="10998-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="10998-105">Někdy se může stát, že se neprojeví změna, a to i v případě, že se změna šíří, ale ukládání do mezipaměti na portálu se nezmění.</span><span class="sxs-lookup"><span data-stu-id="10998-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="10998-106">Pokud je aktivace opožděná, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="10998-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="10998-107">Odhlaste se z portálu Azure a pak se znovu přihlaste.</span><span class="sxs-lookup"><span data-stu-id="10998-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="10998-108">Když aktivujete roli Azure AD nebo roli prostředku Azure, uvidíte fáze aktivace.</span><span class="sxs-lookup"><span data-stu-id="10998-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="10998-109">Po dokončení všech fází uvidíte odkaz odhlásit se.</span><span class="sxs-lookup"><span data-stu-id="10998-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="10998-110">K odhlášení můžete použít tento odkaz. Tato akce vyřeší většinu případů pro zpoždění aktivace.</span><span class="sxs-lookup"><span data-stu-id="10998-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="10998-111">Ve PIM ověřte, že jste uvedeni jako člen role.</span><span class="sxs-lookup"><span data-stu-id="10998-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="10998-112">Pokud aktivujete roli správce Exchange, ujistěte se, že se odhlásíte a zase se přihlásíte.</span><span class="sxs-lookup"><span data-stu-id="10998-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="10998-113">Pokud problém přetrvává, otevřete lístek podpory a vyvolejte ho jako problém.</span><span class="sxs-lookup"><span data-stu-id="10998-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="10998-114">Pokud k centru zabezpečení a dodržování předpisů používáte roli správce Exchange, podívejte se na další krok.</span><span class="sxs-lookup"><span data-stu-id="10998-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="10998-115">Pokud aktivujete roli pro přístup k centru zabezpečení a dodržování předpisů nebo Pokud aktivujete roli správce SharePointu, dojde k některému zpoždění pro aktivaci až pár minut.</span><span class="sxs-lookup"><span data-stu-id="10998-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="10998-116">Jedná se o známý problém a my aktivně pracujeme na řešení tohoto problému s těmito týmy.</span><span class="sxs-lookup"><span data-stu-id="10998-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="10998-117">Další informace najdete tady:</span><span class="sxs-lookup"><span data-stu-id="10998-117">For more information, see:</span></span>

- [<span data-ttu-id="10998-118">Aktivace mých rolí služby Azure AD v PIM</span><span class="sxs-lookup"><span data-stu-id="10998-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="10998-119">Aktivace mých rolí zdrojů Azure v PIM</span><span class="sxs-lookup"><span data-stu-id="10998-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="10998-120">**Po deaktivaci role nebo vypršení platnosti aktivace role nejsou oprávnění odebrána**</span><span class="sxs-lookup"><span data-stu-id="10998-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="10998-121">Když deaktivujete roli ve správě privilegované identity služby Azure AD nebo když vyprší lhůta pro její aktivaci, může dojít k prodlevě, po jejímž uplynutí budete mít přístup.</span><span class="sxs-lookup"><span data-stu-id="10998-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="10998-122">Pokud je deaktivace opožděná, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="10998-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="10998-123">Pokud jste deaktivaci role správce Exchange nebo uplynutím lhůty pro její aktivaci vyprší významné zpoždění před odebráním oprávnění, otevřete lístek podpory a sdělte pracovníkovi podpory, aby vám pomohli poznat lístek s privilegovanou správou přístupu (PAM) v Office o tomto problému.</span><span class="sxs-lookup"><span data-stu-id="10998-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="10998-124">Pokud vypršela lhůta pro aktivaci, ale máte pořád otevřenou relaci prohlížeče, zavřete prohlížeč.</span><span class="sxs-lookup"><span data-stu-id="10998-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="10998-125">Roli můžete dál používat, dokud tuto relaci nezavřete.</span><span class="sxs-lookup"><span data-stu-id="10998-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="10998-126">Jedná se o známý problém a my prohlížíme možnou opravu aktivně odvolat, jakmile vypršela platnost aktivace.</span><span class="sxs-lookup"><span data-stu-id="10998-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="10998-127">Pokud se vaše zpoždění liší od těchto dvou scénářů, otevřete lístek podpory.</span><span class="sxs-lookup"><span data-stu-id="10998-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
