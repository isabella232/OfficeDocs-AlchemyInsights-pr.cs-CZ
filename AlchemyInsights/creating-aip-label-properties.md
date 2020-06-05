---
title: Vytváření zásad popisků AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/03/2020
ms.locfileid: "44568959"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="0515f-102">Vytváření zásad popisků AIP</span><span class="sxs-lookup"><span data-stu-id="0515f-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="0515f-103">Popisky Azure Information Protection(AIP) lze použít s celou řadou dat, která organizace obvykle vytváří a ukládá, od nejnižší klasifikace osobních údajů až po nejvyšší klasifikaci vysoce důvěrných dat.</span><span class="sxs-lookup"><span data-stu-id="0515f-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="0515f-104">Zásady ochrany informací Azure platí pro klasického klienta Azure Information Protection(AIP) a ne na [klienta sjednoceného označování AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="0515f-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="0515f-105">V zásadách AIP můžete nakonfigurovat více prvků, včetně možností, jako jsou:</span><span class="sxs-lookup"><span data-stu-id="0515f-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="0515f-106">Možnost, pro kterou štítek umožní správcům nebo uživatelům klasifikovat a ochranu (volitelné) dokumenty a e-maily</span><span class="sxs-lookup"><span data-stu-id="0515f-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="0515f-107">Možnost vynucení klasifikace při ukládání dokumentů a odesílání e-mailů uživateli</span><span class="sxs-lookup"><span data-stu-id="0515f-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="0515f-108">Možnost automatického označení e-mailové zprávy na základě jejích příloh.</span><span class="sxs-lookup"><span data-stu-id="0515f-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="0515f-109">Možnost řídit, zda se má panel Ochrana informací zobrazit v aplikacích Office</span><span class="sxs-lookup"><span data-stu-id="0515f-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="0515f-110">Další možnosti a informace o zásadách Ochrany informací Azure najdete [v tématu Přehled zásad ochrany informací Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="0515f-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="0515f-111">Další užitečné zdroje týkající se zásad AIP naleznete v tématu:</span><span class="sxs-lookup"><span data-stu-id="0515f-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="0515f-112">Kurz: Konfigurace nastavení zásad Ochrany informací Azure a vytvoření nového popisku</span><span class="sxs-lookup"><span data-stu-id="0515f-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="0515f-113">Konfigurace zásad ochrany informací Azure</span><span class="sxs-lookup"><span data-stu-id="0515f-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="0515f-114">Vytváření a konfigurace popisků citlivosti a jejich zásad</span><span class="sxs-lookup"><span data-stu-id="0515f-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="0515f-115">Návody pro běžné scénáře, které používají Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="0515f-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="0515f-116">Kontrola dokumentace ochrany informací Azure</span><span class="sxs-lookup"><span data-stu-id="0515f-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="0515f-117">Požadavky na azure information protection</span><span class="sxs-lookup"><span data-stu-id="0515f-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="0515f-118">Úvodní kurz pro Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="0515f-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="0515f-119">Stažení klienta Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="0515f-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)