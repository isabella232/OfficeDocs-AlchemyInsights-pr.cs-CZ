---
title: Moderní fakturace e-mailu Azure
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922023"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="10455-102">Fakturace e-mailu v Azure</span><span class="sxs-lookup"><span data-stu-id="10455-102">Email invoicing in Azure</span></span>

<span data-ttu-id="10455-103">Abyste mohli aktualizovat svou e-mailovou fakturu, musíte mít roli vlastníka nebo přispěvatele v fakturačním profilu nebo jeho fakturačním účtu.</span><span class="sxs-lookup"><span data-stu-id="10455-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="10455-104">Jakmile se rozhodnete, že všichni uživatelé s rolí vlastník, přispěvatel, čtenáři a správce faktur v profilu fakturace obdrží svou fakturu v e-mailu.</span><span class="sxs-lookup"><span data-stu-id="10455-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="10455-105">Přihlaste se k [portálu Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="10455-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="10455-106">Vyhledejte **správu nákladů + fakturace**.</span><span class="sxs-lookup"><span data-stu-id="10455-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="10455-107">V horní části stránky vyberte **faktury** a pak vyberte **e-mailová faktura** .</span><span class="sxs-lookup"><span data-stu-id="10455-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="10455-108">Pokud máte několik fakturačních profilů, vyberte profil fakturace a pak vyberte **Přihlásit se**.</span><span class="sxs-lookup"><span data-stu-id="10455-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="10455-109">Vyberte **aktualizovat**.</span><span class="sxs-lookup"><span data-stu-id="10455-109">Select **Update**.</span></span>
6. <span data-ttu-id="10455-110">Pokud máte několik fakturačních profilů, vyberte profil fakturace a pak vyberte **Přihlásit se**.</span><span class="sxs-lookup"><span data-stu-id="10455-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="10455-111">Chcete-li ostatním udělit přístup k zobrazení, stažení a placení faktur, přiřaďte jim roli správce faktur pro fakturační profil MCA nebo MPA.</span><span class="sxs-lookup"><span data-stu-id="10455-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="10455-112">Pokud jste se přihlásili, že budete mít fakturu v e-mailu, uživatelé také získají faktury v e-mailu.</span><span class="sxs-lookup"><span data-stu-id="10455-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="10455-113">Přihlaste se k [portálu Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="10455-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="10455-114">Vyhledejte **správu nákladů + fakturace**.</span><span class="sxs-lookup"><span data-stu-id="10455-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="10455-115">Vyberte **profily pro fakturaci** z levé strany.</span><span class="sxs-lookup"><span data-stu-id="10455-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="10455-116">V seznamu profily faktur vyberte profil fakturace, pro který chcete přiřadit roli správce faktury.</span><span class="sxs-lookup"><span data-stu-id="10455-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="10455-117">V levé části vyberte **řízení přístupu (IAM)** a potom v horní části stránky vyberte **Přidat** .</span><span class="sxs-lookup"><span data-stu-id="10455-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="10455-118">V rozevíracím seznamu role vyberte **správce faktur**.</span><span class="sxs-lookup"><span data-stu-id="10455-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="10455-119">Zadejte e-mailovou adresu uživatele, kterému chcete udělit přístup.</span><span class="sxs-lookup"><span data-stu-id="10455-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="10455-120">Kliknutím na **Uložit** roli přiřadíte.</span><span class="sxs-lookup"><span data-stu-id="10455-120">Select **Save** to assign the role.</span></span>
