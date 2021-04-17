---
title: Moderní e-mailová fakturace Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820819"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="0e7fe-102">E-mailová fakturace v Azure</span><span class="sxs-lookup"><span data-stu-id="0e7fe-102">Email invoicing in Azure</span></span>

<span data-ttu-id="0e7fe-103">Abyste mohli aktualizovat předvolby e-mailové fakturace, musíte mít na fakturačním profilu nebo na jeho fakturačním účtu roli vlastníka nebo přispěvatele.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="0e7fe-104">Jakmile to odsouhlasíte, všichni uživatelé s rolí vlastníka, přispěvatele, čtenáře a správce faktur na fakturačním profilu dostanou fakturu tohoto profilu e-mailem.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="0e7fe-105">Přihlaste se na [portál Microsoft Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="0e7fe-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="0e7fe-106">Vyhledejte položku **Správa nákladů + fakturace**.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="0e7fe-107">Vyberte **Faktury** na levé straně a v horní části stránky pak vyberte možnost **Poslat fakturu e-mailem**.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="0e7fe-108">Pokud máte fakturačních profilů víc, vyberte některý z nich a pak vyberte **Vyjádřit souhlas**.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="0e7fe-109">Vyberte **Aktualizovat**.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-109">Select **Update**.</span></span>
6. <span data-ttu-id="0e7fe-110">Pokud máte fakturačních profilů víc, vyberte některý z nich a pak vyberte **Vyjádřit souhlas**.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="0e7fe-111">Ostatním uživatelům můžete udělit přístup k zobrazování, stahování a placení faktur tím, že jim přiřadíte roli správce faktur pro fakturační profil MCA nebo MPA.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="0e7fe-112">Pokud jste odsouhlasili, že faktury budete dostávat e-mailem, i uživatelům budou chodit faktury e-mailem.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="0e7fe-113">Přihlaste se na [portál Microsoft Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="0e7fe-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="0e7fe-114">Vyhledejte položku **Správa nákladů + fakturace**.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="0e7fe-115">Vyberte **Fakturační profily** na levé straně.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="0e7fe-116">V seznamu fakturačních profilů vyberte fakturační profil, ke kterému chcete přiřadit roli správce faktur.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="0e7fe-117">Vyberte **Řízení přístupu (systém IAM)** na levé straně a pak vyberte **Přidat** v horní části stránky.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="0e7fe-118">V rozevíracím seznamu Role vyberte **Správce faktur**.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="0e7fe-119">Zadejte e-mailovou adresu uživatele, kterému chcete udělit přístup.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="0e7fe-120">Výběrem možnosti **Uložit** roli přiřadíte.</span><span class="sxs-lookup"><span data-stu-id="0e7fe-120">Select **Save** to assign the role.</span></span>
