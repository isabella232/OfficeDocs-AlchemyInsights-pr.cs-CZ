---
title: Nastavení DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808700"
---
# <a name="setup-dkim"></a><span data-ttu-id="698d8-102">Nastavení DKIM</span><span class="sxs-lookup"><span data-stu-id="698d8-102">Setup DKIM</span></span>

<span data-ttu-id="698d8-103">Kompletní pokyny ke konfiguraci DKIM pro vlastní domény v Microsoft 365 [najdete tady](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="698d8-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="698d8-104">Pro **každou** vlastní doménu musíte vytvořit **dva** záznamy CNAME DKIM v hostitelské službě DNS vaší domény (obvykle doménového registrátora).</span><span class="sxs-lookup"><span data-stu-id="698d8-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="698d8-105">Například contoso.com a fourthcoffee.com vyžadují čtyři DKIM záznamy CNAME: dvě pro contoso.com a dva pro fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="698d8-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="698d8-106">Záznamy CNAME DKIM pro **každou** vlastní doménu používají následující formáty:</span><span class="sxs-lookup"><span data-stu-id="698d8-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="698d8-107">**Název hostitele**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="698d8-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="698d8-108">**Odkazuje na adresu nebo hodnotu**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="698d8-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="698d8-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="698d8-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="698d8-110">**Název hostitele**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="698d8-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="698d8-111">**Odkazuje na adresu nebo hodnotu**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="698d8-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="698d8-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="698d8-112">**TTL**: 3600</span></span>

   <span data-ttu-id="698d8-113">\<DomainGUID\> je text nalevo od `.mail.protection.outlook.com` přizpůsobeného záznamu MX pro vlastní doménu (třeba `contoso-com` pro doménu contoso.com).</span><span class="sxs-lookup"><span data-stu-id="698d8-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="698d8-114">\<InitialDomain\> je doména, kterou jste použili při registraci k Microsoft 365 (například contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="698d8-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="698d8-115">Po vytvoření záznamů CNAME pro vlastní domény postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="698d8-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="698d8-116">a.</span><span class="sxs-lookup"><span data-stu-id="698d8-116">a.</span></span> <span data-ttu-id="698d8-117">[Přihlaste se k Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomocí svého pracovního nebo školního účtu.</span><span class="sxs-lookup"><span data-stu-id="698d8-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="698d8-118">b.</span><span class="sxs-lookup"><span data-stu-id="698d8-118">b.</span></span> <span data-ttu-id="698d8-119">V levém horním rohu vyberte ikonu spouštěče aplikací a zvolte **Správce**.</span><span class="sxs-lookup"><span data-stu-id="698d8-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="698d8-120">c.</span><span class="sxs-lookup"><span data-stu-id="698d8-120">c.</span></span> <span data-ttu-id="698d8-121">V navigačním panelu v levém dolním rohu rozbalte položku **správce** a zvolte **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="698d8-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="698d8-122">d.</span><span class="sxs-lookup"><span data-stu-id="698d8-122">d.</span></span> <span data-ttu-id="698d8-123">Přejděte na **Protection**  >  **DKIM**ochrany.</span><span class="sxs-lookup"><span data-stu-id="698d8-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="698d8-124">e.</span><span class="sxs-lookup"><span data-stu-id="698d8-124">e.</span></span> <span data-ttu-id="698d8-125">Vyberte doménu a pak **pomocí DKIM podpisů pro tuto doménu**vyberte **Povolit** .</span><span class="sxs-lookup"><span data-stu-id="698d8-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="698d8-126">Tento krok opakujte pro každou vlastní doménu.</span><span class="sxs-lookup"><span data-stu-id="698d8-126">Repeat this step for each custom domain.</span></span>
