---
title: Převod vlastnictví fakturace v Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922029"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="d90e6-102">Převod vlastnictví fakturace v Azure</span><span class="sxs-lookup"><span data-stu-id="d90e6-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="d90e6-103">Přihlaste se k [portálu Azure](https://portal.azure.com/) jako správce fakturačního účtu, který má předplatné, které chcete přenést.</span><span class="sxs-lookup"><span data-stu-id="d90e6-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="d90e6-104">Pokud si nejste jistí, jestli jste správcem, nebo pokud potřebujete zjistit, kdo je, přečtěte si článek [určení správce fakturace účtu](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="d90e6-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="d90e6-105">Vyhledávání ve **správě nákladů + fakturace**</span><span class="sxs-lookup"><span data-stu-id="d90e6-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="d90e6-106">Vyberte možnost **předplatná** z levého podokna.</span><span class="sxs-lookup"><span data-stu-id="d90e6-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="d90e6-107">V závislosti na Accessu možná budete muset vybrat rozsah fakturace a potom **předplatné** nebo **předplatné Azure**.</span><span class="sxs-lookup"><span data-stu-id="d90e6-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="d90e6-108">Vyberte **převést vlastnictví fakturace** pro předplatné, které chcete přenést.</span><span class="sxs-lookup"><span data-stu-id="d90e6-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="d90e6-109">Zadejte e-mailovou adresu uživatele, který je správcem fakturace účtu, který bude novým vlastníkem předplatného, a pak vyberte **Odeslat žádost o odeslání**</span><span class="sxs-lookup"><span data-stu-id="d90e6-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="d90e6-110">Uživatel obdrží e-mailovou zprávu s pokyny pro kontrolu žádosti o převod.</span><span class="sxs-lookup"><span data-stu-id="d90e6-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="d90e6-111">Pokud chcete žádost o převod schválit, uživatel v e-mailu vybere odkaz a postupujte podle pokynů.</span><span class="sxs-lookup"><span data-stu-id="d90e6-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="d90e6-112">**Poznámka** : Pokud převedete vlastnictví svého předplatného na účet uživatele v jiném Azure AD tenantovi, budou trvale odebrány všechny úlohy [řízení přístupu založené na rolích (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)pro správu zdrojů.</span><span class="sxs-lookup"><span data-stu-id="d90e6-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="d90e6-113">Jenom nový vlastník bude mít přístup ke správě zdrojů v předplatném.</span><span class="sxs-lookup"><span data-stu-id="d90e6-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="d90e6-114">Další informace najdete v tématu [Převod předplatného na uživatele v jiném Azure AD tenantovi](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d90e6-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="d90e6-115">**Doporučené dokumenty**</span><span class="sxs-lookup"><span data-stu-id="d90e6-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="d90e6-116">Převod vlastnictví účtu Azure na jiný účet</span><span class="sxs-lookup"><span data-stu-id="d90e6-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="d90e6-117">O převodu vlastnictví fakturace pro předplatné Azure</span><span class="sxs-lookup"><span data-stu-id="d90e6-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="d90e6-118">Přenášení Visual studia, partnera sítě Microsoft (MPN) a platby průběžně</span><span class="sxs-lookup"><span data-stu-id="d90e6-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="d90e6-119">Časté otázky k převodu vlastnictví</span><span class="sxs-lookup"><span data-stu-id="d90e6-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="d90e6-120">Řešení problémů s převodem vlastnictví</span><span class="sxs-lookup"><span data-stu-id="d90e6-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
