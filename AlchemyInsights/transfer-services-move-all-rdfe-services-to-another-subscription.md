---
title: Přenos služeb – přesunutí všech služeb RDFE do jiného předplatného
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691977"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="61c37-102">Přenos služeb – přesunutí všech služeb RDFE do jiného předplatného</span><span class="sxs-lookup"><span data-stu-id="61c37-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="61c37-103">**Přesunutí zdrojů**</span><span class="sxs-lookup"><span data-stu-id="61c37-103">**Move resources**</span></span>

<span data-ttu-id="61c37-104">Prostředky Azure se dají přesunout do jiného předplatného Azure nebo skupiny prostředků pod stejným předplatným pomocí Azure Portal, Azure PowerShellu, Azure CLI nebo REST API pro přesouvání prostředků.</span><span class="sxs-lookup"><span data-stu-id="61c37-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="61c37-105">Než budete moct přesunout zdroje, přečtěte si téma:</span><span class="sxs-lookup"><span data-stu-id="61c37-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="61c37-106">Kontrolní seznam před přesunutím zdrojů</span><span class="sxs-lookup"><span data-stu-id="61c37-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="61c37-107">Služby, které lze přesunout</span><span class="sxs-lookup"><span data-stu-id="61c37-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="61c37-108">Jak ověřit přesunutí</span><span class="sxs-lookup"><span data-stu-id="61c37-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="61c37-109">Přesunutí pokynů pro služby</span><span class="sxs-lookup"><span data-stu-id="61c37-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="61c37-110">Pokud chcete přesunout existující zdroje do jiné skupiny zdrojů nebo předplatného, můžete použít:</span><span class="sxs-lookup"><span data-stu-id="61c37-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="61c37-111">Portál Azure</span><span class="sxs-lookup"><span data-stu-id="61c37-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="61c37-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="61c37-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="61c37-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="61c37-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="61c37-114">REST API</span><span class="sxs-lookup"><span data-stu-id="61c37-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="61c37-115">Kurz: [přesunutí zdrojů Azure do jiné skupiny zdrojů nebo předplatného](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="61c37-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="61c37-116">**Poradce při potížích se správcem prostředků Azure**</span><span class="sxs-lookup"><span data-stu-id="61c37-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="61c37-117">Informace o některých běžných chybách nasazení Azure a získávání informací pro jejich řešení najdete v článcích níže.</span><span class="sxs-lookup"><span data-stu-id="61c37-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="61c37-118">Pokud kód chyby chyby nasazení nemůžete najít, přečtěte si téma [vyhledání kódu chyby](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="61c37-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="61c37-119">Řešení chyb nasazení</span><span class="sxs-lookup"><span data-stu-id="61c37-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="61c37-120">Řešení potíží při přesouvání prostředků Azure do nové skupiny zdrojů nebo předplatného</span><span class="sxs-lookup"><span data-stu-id="61c37-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="61c37-121">Uvědomte si, že pokud si přejete upgradovat předplatné Azure, třeba přepnout z bezplatného na to-to-do, budete muset předplatné převést.</span><span class="sxs-lookup"><span data-stu-id="61c37-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="61c37-122">Pokud chcete upgradovat bezplatnou zkušební verzi, přečtěte si článek [upgrade bezplatného zkušebního předplatného společnosti Microsoft](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)a vyzkoušejte si předplatné Azure.</span><span class="sxs-lookup"><span data-stu-id="61c37-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="61c37-123">Pokud chcete změnit účet s účtem s účtem, přečtěte si článek [Změna předplatného služby Azure Pay-as-to-go na jinou nápovědu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="61c37-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="61c37-124">**Přidání nebo přidružení předplatného Azure ke svému tenantovi Azure Active Directory:**</span><span class="sxs-lookup"><span data-stu-id="61c37-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="61c37-125">Přihlaste se a vyberte předplatné, které chcete použít na [stránce Předplatná na portálu Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="61c37-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="61c37-126">Vyberte **změnit adresář**.</span><span class="sxs-lookup"><span data-stu-id="61c37-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="61c37-127">Zkontrolujte všechna zobrazená upozornění a pak vyberte **změnit**.</span><span class="sxs-lookup"><span data-stu-id="61c37-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="61c37-128">U předplatného se změní adresář a zobrazí se zpráva o úspěšném dokončení.</span><span class="sxs-lookup"><span data-stu-id="61c37-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="61c37-129">Pomocí přepínače *adresáře* přejděte do nového adresáře.</span><span class="sxs-lookup"><span data-stu-id="61c37-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="61c37-130">Zobrazení obsahu může trvat až 10 minut.</span><span class="sxs-lookup"><span data-stu-id="61c37-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="61c37-131">**Doporučené dokumenty**</span><span class="sxs-lookup"><span data-stu-id="61c37-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="61c37-132">Převod vlastnictví předplatného Azure</span><span class="sxs-lookup"><span data-stu-id="61c37-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="61c37-133">Přesunutí zdrojů do nové skupiny zdrojů nebo do nového předplatného</span><span class="sxs-lookup"><span data-stu-id="61c37-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="61c37-134">Správa zdrojů pomocí Azure Portal</span><span class="sxs-lookup"><span data-stu-id="61c37-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
