---
title: Vytváření zásad AIP štítků
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732168"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="d2c6c-102">Vytváření zásad AIP štítků</span><span class="sxs-lookup"><span data-stu-id="d2c6c-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="d2c6c-103">Popisky Azure Information Protection (AIP) se dají používat s celou oblastí dat, kterou organizace obvykle vytváří a ukládá z nižší klasifikace osobních údajů do nejvyšší klasifikace vysoce důvěrných dat.</span><span class="sxs-lookup"><span data-stu-id="d2c6c-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="d2c6c-104">Zásady ochrany informací Azure se týkají klasického klienta Azure Information Protection (AIP) a nikoli  [AIP klienta jednotného značení](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="d2c6c-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="d2c6c-105">V zásadách AIP můžete nakonfigurovat více prvků, mezi které patří:</span><span class="sxs-lookup"><span data-stu-id="d2c6c-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="d2c6c-106">Možnost, pro kterou bude popisek umožnit správcům nebo uživatelům klasifikovat a zamknout (volitelné) dokumenty a e-maily</span><span class="sxs-lookup"><span data-stu-id="d2c6c-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="d2c6c-107">Možnost pro vynucení klasifikace při ukládání dokumentů a odesílání e-mailů</span><span class="sxs-lookup"><span data-stu-id="d2c6c-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="d2c6c-108">Možnost, která automaticky označí e-mailovou zprávu podle příloh.</span><span class="sxs-lookup"><span data-stu-id="d2c6c-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="d2c6c-109">Možnost určení, jestli se v aplikacích Office zobrazuje panel ochrany informací</span><span class="sxs-lookup"><span data-stu-id="d2c6c-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="d2c6c-110">Další možnosti a informace o zásadách ochrany informací Azure naleznete v tématu: [Přehled zásad ochrany informací Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="d2c6c-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="d2c6c-111">Další užitečné materiály týkající se zásad AIP naleznete v tématech:</span><span class="sxs-lookup"><span data-stu-id="d2c6c-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="d2c6c-112">Kurz: Konfigurace nastavení zásad ochrany informací Azure a vytvoření nového štítku</span><span class="sxs-lookup"><span data-stu-id="d2c6c-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="d2c6c-113">Konfigurace zásad ochrany informací Azure</span><span class="sxs-lookup"><span data-stu-id="d2c6c-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="d2c6c-114">Vytvoření a konfigurace popisků utajení a jejich zásad</span><span class="sxs-lookup"><span data-stu-id="d2c6c-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="d2c6c-115">Návody pro běžné scénáře používající službu Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="d2c6c-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="d2c6c-116">Přečtěte si dokumentaci k Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="d2c6c-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="d2c6c-117">Požadavky na ochranu informací Azure</span><span class="sxs-lookup"><span data-stu-id="d2c6c-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="d2c6c-118">Rychlý kurz pro rychlé zahájení ochrany informací Azure</span><span class="sxs-lookup"><span data-stu-id="d2c6c-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="d2c6c-119">Stáhnout klienta ochrany informací v Azure</span><span class="sxs-lookup"><span data-stu-id="d2c6c-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)