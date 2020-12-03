---
title: Odstranit tenanta
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564418"
---
# <a name="delete-tenant"></a><span data-ttu-id="0e0d9-102">Odstranit tenanta</span><span class="sxs-lookup"><span data-stu-id="0e0d9-102">Delete tenant</span></span>

<span data-ttu-id="0e0d9-103">Pokud chcete odstranit Azure AD, zkontrolujte:</span><span class="sxs-lookup"><span data-stu-id="0e0d9-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="0e0d9-104">Jste globálním správcem adresáře.</span><span class="sxs-lookup"><span data-stu-id="0e0d9-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="0e0d9-105">Nejste přihlášeni pomocí účtu, který má výchozí adresář, jako je třeba contoso.onmicrosoft.com, v přihlášeném účtu, například admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="0e0d9-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="0e0d9-106">Před odstraněním odeberte všechny aktivní aplikace v adresáři.</span><span class="sxs-lookup"><span data-stu-id="0e0d9-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="0e0d9-107">Pokud chcete odebrat aktivní aplikace, přejděte na registrace aplikací a odeberte stávající aplikace.</span><span class="sxs-lookup"><span data-stu-id="0e0d9-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="0e0d9-108">Žádné aktivní předplatná pro žádné služby Microsoft Online Services, jako je Microsoft Azure, Office 365 nebo Azure AD Premium, přidružené k adresáři.</span><span class="sxs-lookup"><span data-stu-id="0e0d9-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="0e0d9-109">Převeďte svoje předplatné nebo urychlení zrušení aktivních předplatných prostřednictvím podpory Azure a fakturace.</span><span class="sxs-lookup"><span data-stu-id="0e0d9-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="0e0d9-110">Přečtěte si další informace o zrušení předplatného Office 365 a Azure.</span><span class="sxs-lookup"><span data-stu-id="0e0d9-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="0e0d9-111">Pokyny k přidružení nebo přidání existujícího předplatného k tenantovi najdete v článku [přidružení nebo přidání předplatného Azure ke svému Tenantovi Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="0e0d9-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="0e0d9-112">Žádná aktivní licence neexistuje.</span><span class="sxs-lookup"><span data-stu-id="0e0d9-112">There are no Active license.</span></span> <span data-ttu-id="0e0d9-113">Pokud chcete licence odebrat, přečtěte si [článek Jak odebrat předplatné a odebrat licenci](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="0e0d9-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="0e0d9-114">Při pokusu o odstranění Azure AD se v adresáři nevyskytují žádné další aktivní uživatele.</span><span class="sxs-lookup"><span data-stu-id="0e0d9-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="0e0d9-115">Odeberte také všechny ostatní aktivní uživatele a všechny závislosti v názvu vlastní domény v klientovi budou rovněž odebrány, například uživatelé vytvoøeni pomocí admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="0e0d9-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="0e0d9-116">Podrobnější pokyny:</span><span class="sxs-lookup"><span data-stu-id="0e0d9-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="0e0d9-117">Odstranění "Azure Active Directory" nebo "předplatná", viz [odstranění služby Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)</span><span class="sxs-lookup"><span data-stu-id="0e0d9-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="0e0d9-118">Odebrání aplikací v adresáři: Přečtěte si článek [odebrání aplikací](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="0e0d9-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
