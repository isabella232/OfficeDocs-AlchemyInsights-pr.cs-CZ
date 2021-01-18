---
title: Přiřazení skupin k roli Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884912"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="5fd7c-102">Přiřazení skupin k roli Azure AD</span><span class="sxs-lookup"><span data-stu-id="5fd7c-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="5fd7c-103">Pokud chcete skupině Azure AD s zdrojem oprávnění v Azure AD přiřadit roli Azure AD, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="5fd7c-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="5fd7c-104">Vytvořit novou skupinu vytvoří novou skupinu:</span><span class="sxs-lookup"><span data-stu-id="5fd7c-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="5fd7c-105">a.</span><span class="sxs-lookup"><span data-stu-id="5fd7c-105">a.</span></span> <span data-ttu-id="5fd7c-106">Přihlaste se do centra pro správu Azure AD s oprávněním **správce rolí** nebo **globálního správce** .</span><span class="sxs-lookup"><span data-stu-id="5fd7c-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="5fd7c-107">b.</span><span class="sxs-lookup"><span data-stu-id="5fd7c-107">b.</span></span> <span data-ttu-id="5fd7c-108">Vyberte **skupiny služby Azure Active Directory > > všechny skupiny > novou skupinu**.</span><span class="sxs-lookup"><span data-stu-id="5fd7c-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="5fd7c-109">c.</span><span class="sxs-lookup"><span data-stu-id="5fd7c-109">c.</span></span> <span data-ttu-id="5fd7c-110">Vytvořte skupinu.</span><span class="sxs-lookup"><span data-stu-id="5fd7c-110">Create the group.</span></span>

2. <span data-ttu-id="5fd7c-111">Přiřaďte roli skupině při vytváření skupiny nebo po vytvoření skupiny.</span><span class="sxs-lookup"><span data-stu-id="5fd7c-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="5fd7c-112">a.</span><span class="sxs-lookup"><span data-stu-id="5fd7c-112">a.</span></span> <span data-ttu-id="5fd7c-113">Pokud chcete skupině přiřadit roli při vytváření skupiny, přepněte na přepínač **role služby Azure AD do skupiny** a vytvořte skupinu.</span><span class="sxs-lookup"><span data-stu-id="5fd7c-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="5fd7c-114">b.</span><span class="sxs-lookup"><span data-stu-id="5fd7c-114">b.</span></span> <span data-ttu-id="5fd7c-115">Pokud chcete přiřadit roli skupině po jejím vytvoření, přejděte na kartu **přiřazené role** pro nově vytvořenou skupinu a přiřaďte roli skupině.</span><span class="sxs-lookup"><span data-stu-id="5fd7c-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="5fd7c-116">**Správa členství ve skupině, která je přiřazená k roli Azure AD**</span><span class="sxs-lookup"><span data-stu-id="5fd7c-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="5fd7c-117">Abyste předešli zvýšení oprávnění, můžou ve výchozím nastavení měnit členství ve skupině, která je přiřazená k roli, jenom správcům rolí a globálních správcům.</span><span class="sxs-lookup"><span data-stu-id="5fd7c-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="5fd7c-118">Mohou však zvolit přiřazení vlastníka takové skupiny a delegovat tento úkol.</span><span class="sxs-lookup"><span data-stu-id="5fd7c-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="5fd7c-119">Další informace o přiřazování cloudových skupin k rolím Azure AD najdete v tématu [přiřazení rolí služby AD ke skupině cloudu](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="5fd7c-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="5fd7c-120">Další informace o rolích řešení potíží přiřazených ke skupinám cloudu najdete v tématu [řešení potíží s rolemi přiřazenými cloudovým skupinám](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="5fd7c-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





