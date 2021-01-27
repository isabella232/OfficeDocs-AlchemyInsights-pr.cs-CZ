---
title: Kontroly Accessu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7767"
ms.openlocfilehash: b2ba50c4f8e667f81b638ba480fa846e149c3d43
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014745"
---
# <a name="access-reviews"></a><span data-ttu-id="03257-102">Kontroly Accessu</span><span class="sxs-lookup"><span data-stu-id="03257-102">Access reviews</span></span>

1. <span data-ttu-id="03257-103">**Povolení recenzí Accessu**: při vytvoření nového balíčku Accessu nebo úpravě existujícího balíčku Accessu můžete povolit kontroly.</span><span class="sxs-lookup"><span data-stu-id="03257-103">**Enable Access Reviews**: You can enable reviews when you create a new access package or edit an existing access package.</span></span> <span data-ttu-id="03257-104">[Vytvoření kontroly Accessu balíčku Accessu v Azure AD – Správa nároků](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) popisuje, jak povolit Access zkontrolovat balíčky Accessu.</span><span class="sxs-lookup"><span data-stu-id="03257-104">[Create an access review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to enable access reviews of access packages.</span></span>

1. <span data-ttu-id="03257-105">**Kontrola přístupu**: Správa oprávnění Azure AD zjednodušuje způsob, jakým podniky spravují přístup ke skupinám, aplikacím a sharepointovým webům.</span><span class="sxs-lookup"><span data-stu-id="03257-105">**Review Access**: Azure AD entitlement management simplifies how enterprises manage access to groups, applications, and SharePoint sites.</span></span> <span data-ttu-id="03257-106">[Kontrola přístupu k balíčku Accessu v Azure AD managementu](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) : popisuje, jak udělat kontroly Accessu pro další uživatele, kteří jsou přiřazeni k balíčku Accessu jako vyhrazený revidující.</span><span class="sxs-lookup"><span data-stu-id="03257-106">[Review access of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to perform access reviews for other users that are assigned to an access package as a designated reviewer.</span></span>

1. <span data-ttu-id="03257-107">**Zkontrolujte přístup sami**: [vlastní kontrola balíčku Accessu v Azure AD – Správa nároků](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) popisuje, jak uživatel provede vlastní kontrolu přiřazených balíčků pro Access.</span><span class="sxs-lookup"><span data-stu-id="03257-107">**Review Access for Yourself**: [Self-review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) describes how a user does a self-review of their assigned access package(s).</span></span>

1. <span data-ttu-id="03257-108">Ve většině případů budou koncoví uživatelé hledat, dokud nečekají na odpověď na **panelu přístupu**.</span><span class="sxs-lookup"><span data-stu-id="03257-108">In most cases, end users will find a review pending their response in the **Access Panel**.</span></span> <span data-ttu-id="03257-109">Tento postup platí jenom pro recenze skupin a aplikací, ne na role.</span><span class="sxs-lookup"><span data-stu-id="03257-109">This is only applicable to reviews of Groups and Applications, not Roles.</span></span> <span data-ttu-id="03257-110">U všech přístupových přehledů rolí musí koncoví uživatelé provést revizi přechodem na správu privilegované identity Azure AD.</span><span class="sxs-lookup"><span data-stu-id="03257-110">For all Access Reviews of roles, end users must navigate to Azure AD Privileged Identity Management (PIM) to complete their review.</span></span>

    1. <span data-ttu-id="03257-111">Přihlaste se k portálu Azure.</span><span class="sxs-lookup"><span data-stu-id="03257-111">Logon to the Azure portal.</span></span>
    2. <span data-ttu-id="03257-112">Přejděte na Azure AD PIM.</span><span class="sxs-lookup"><span data-stu-id="03257-112">Navigate to Azure AD PIM.</span></span>
    3. <span data-ttu-id="03257-113">V levém navigačním podokně vyberte možnost **úkoly**-  >  **Kontrola přístupu**.</span><span class="sxs-lookup"><span data-stu-id="03257-113">In the left navigation pane, select **Tasks** > **Review access**.</span></span>
    
<span data-ttu-id="03257-114">Další informace najdete tady:</span><span class="sxs-lookup"><span data-stu-id="03257-114">For more information, see:</span></span>

- [<span data-ttu-id="03257-115">Provedení kontroly přístupu mých rolí adresáře služby Azure AD v PIM </span><span class="sxs-lookup"><span data-stu-id="03257-115">Perform an access review of my Azure AD directory roles in PIM </span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-perform-security-review/)
- [<span data-ttu-id="03257-116">Provedení kontroly přístupu mých rolí zdrojů Azure v PIM</span><span class="sxs-lookup"><span data-stu-id="03257-116">Perform an access review of my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-perform-access-review/)