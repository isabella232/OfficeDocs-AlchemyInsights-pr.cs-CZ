---
title: Povolit správu nákladů
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676958"
---
# <a name="enable-cost-management"></a><span data-ttu-id="42513-102">Povolit správu nákladů</span><span class="sxs-lookup"><span data-stu-id="42513-102">Enable cost management</span></span>

<span data-ttu-id="42513-103">**Co znamená, že náklady jsou pro vaši organizaci zakázané?**</span><span class="sxs-lookup"><span data-stu-id="42513-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="42513-104">Organizace používající podnikové smlouvy (EA) nebo účty Microsoft Customer Agreement (MCA) mohou zakázat přístup k informacím o nákladech a cenách.</span><span class="sxs-lookup"><span data-stu-id="42513-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="42513-105">Po přihlášení k Azure Portal mohou používat API pro fakturaci k programovému získávání faktur (po obdržení) a podrobností o využití.</span><span class="sxs-lookup"><span data-stu-id="42513-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="42513-106">**Jak povolit dalším uživatelům přístup k fakturám**</span><span class="sxs-lookup"><span data-stu-id="42513-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="42513-107">Přejděte na **okno předplatná** na portálu Azure.</span><span class="sxs-lookup"><span data-stu-id="42513-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="42513-108">Vyberte **faktury** a pak **přístup k fakturám**.</span><span class="sxs-lookup"><span data-stu-id="42513-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="42513-109">Zapnutím Accessu a uložením změn umožníte uživatelům v rolích s rozsahem předplatného stáhnout faktury.</span><span class="sxs-lookup"><span data-stu-id="42513-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="42513-110">Správce účtu může také nakonfigurovat, aby faktury poslal e-mailem.</span><span class="sxs-lookup"><span data-stu-id="42513-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="42513-111">Další informace najdete v tématu [získání faktury v e-mailu](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="42513-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="42513-112">**Přidání uživatelů do role čtečka fakturace**</span><span class="sxs-lookup"><span data-stu-id="42513-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="42513-113">Přejděte na **okno předplatná** na portálu Azure.</span><span class="sxs-lookup"><span data-stu-id="42513-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="42513-114">Vyberte **řízení přístupu (IAM)** a potom klikněte na **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="42513-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="42513-115">Na stránce **Vybrat roli** zvolte **čtečka fakturace** .</span><span class="sxs-lookup"><span data-stu-id="42513-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="42513-116">Zadejte e-mail uživatele, kterého chcete pozvat, a kliknutím na **OK** pozvánku odešlete.</span><span class="sxs-lookup"><span data-stu-id="42513-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="42513-117">Postupujte podle pokynů v e-mailu pozvat pro přihlášení jako čtečku fakturace.</span><span class="sxs-lookup"><span data-stu-id="42513-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="42513-118">Další informace najdete v článku [udělení přístupu k fakturaci](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="42513-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="42513-119">**Doporučené dokumenty**</span><span class="sxs-lookup"><span data-stu-id="42513-119">**Recommended documents**</span></span>

- [<span data-ttu-id="42513-120">Povolení zobrazení DA a AO na portálu EA</span><span class="sxs-lookup"><span data-stu-id="42513-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="42513-121">Náklady zahrnuté v řízení nákladů</span><span class="sxs-lookup"><span data-stu-id="42513-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="42513-122">Podporované nabídky Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="42513-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="42513-123">Zkontrolovat náklady v analýze nákladů</span><span class="sxs-lookup"><span data-stu-id="42513-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="42513-124">Poskytnutí přístupu k fakturačním informacím</span><span class="sxs-lookup"><span data-stu-id="42513-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="42513-125">Kontrola přístupu ke Smlouvě o zákaznících Microsoftu</span><span class="sxs-lookup"><span data-stu-id="42513-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






