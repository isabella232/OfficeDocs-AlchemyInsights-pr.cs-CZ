---
title: Virtuální konfigurace s doménovým službám AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884976"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="502ee-102">Virtuální konfigurace s doménovým službám AAD</span><span class="sxs-lookup"><span data-stu-id="502ee-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="502ee-103">Virtuální konfigurace s doménou AAD zahrnuje následující kroky:</span><span class="sxs-lookup"><span data-stu-id="502ee-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="502ee-104">Kontrola stavu vaší domény na Azure Portalu https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="502ee-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="502ee-105">Kontrola NSG pravidel, která blokují porty potřebné k synchronizaci v Azure AD Domain Services na portálu https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="502ee-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="502ee-106">Ujistěte se, že je vaše virtuální síť nasazená ve stejné oblasti Azure jako doména spravovaná službou Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="502ee-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="502ee-107">Ujistěte se, že nemáte ve virtuální síti k dispozici stejnou doménu s názvem domény.</span><span class="sxs-lookup"><span data-stu-id="502ee-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="502ee-108">Další podrobnosti o zvažování návrhu pro podporu služby DNS Virtual Network najdete v tématu [zvážení virtuální sítě](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="502ee-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

