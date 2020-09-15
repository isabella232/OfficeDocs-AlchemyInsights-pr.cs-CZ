---
title: Přidání externích uživatelů do distribuční skupiny
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663506"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="e4a8d-102">Přidání externích uživatelů do distribuční skupiny</span><span class="sxs-lookup"><span data-stu-id="e4a8d-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="e4a8d-103">Přidání externího kontaktu do distribuční skupiny (DG) je proces se dvěma kroky:</span><span class="sxs-lookup"><span data-stu-id="e4a8d-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="e4a8d-104">Vytvoření e-mailového kontaktu pro externího uživatele:</span><span class="sxs-lookup"><span data-stu-id="e4a8d-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="e4a8d-105">V centru pro správu přejděte na **Users**  >  stránku[Kontakty](https://admin.microsoft.com/adminportal/home#/Contact) pro uživatele.</span><span class="sxs-lookup"><span data-stu-id="e4a8d-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="e4a8d-106">Vyberte **Přidat kontakt**.</span><span class="sxs-lookup"><span data-stu-id="e4a8d-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="e4a8d-107">Zadejte informace o kontaktu a vyberte **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="e4a8d-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="e4a8d-108">Přidejte poštovní kontakt do svého DISTRIBUČNÍho systému:</span><span class="sxs-lookup"><span data-stu-id="e4a8d-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="e4a8d-109">V centru pro správu přejděte na stránku skupiny **skupiny**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="e4a8d-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="e4a8d-110">Najděte distribuční položku, ke které chcete externího uživatele přidat, a vyberte ji a otevřete tak dialogové okno Upravit.</span><span class="sxs-lookup"><span data-stu-id="e4a8d-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="e4a8d-111">Na kartě **Členové** vyberte **Zobrazit všechny a spravovat členy**.</span><span class="sxs-lookup"><span data-stu-id="e4a8d-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="e4a8d-112">Vyberte **přidat členy**.</span><span class="sxs-lookup"><span data-stu-id="e4a8d-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="e4a8d-113">Vyberte kontakt pošty, který jste vytvořili v předchozím kroku, a pak vyberte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="e4a8d-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="e4a8d-114">Pokud po provedení těchto kroků nebudou externí uživatelé moct posílat e-maily distribuční skupině nebo nedostávat e-maily, může to být, když je distribuční společnost označena tak, že povolí pouze e-maily od interních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="e4a8d-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="e4a8d-115">Můžete zkontrolovat tuto konfiguraci a opravit ji [podle pokynů.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="e4a8d-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="e4a8d-116">**Poznámka:** Tyto pokyny se nevztahují, pokud typ vaší skupiny je "skupina Microsoft 365" místo "distribuční skupina".</span><span class="sxs-lookup"><span data-stu-id="e4a8d-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="e4a8d-117">V tom případě můžete externího uživatele přidat přímo do skupiny z Outlooku.</span><span class="sxs-lookup"><span data-stu-id="e4a8d-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="e4a8d-118">Podrobné informace o skupinách společností Microsoft 365 a pokyny pro přidání externích hostů najdete v [tomto článku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="e4a8d-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  