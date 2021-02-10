---
title: Problém se skupinami zabezpečení
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177386"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="5173d-102">Problém se skupinami zabezpečení</span><span class="sxs-lookup"><span data-stu-id="5173d-102">Issue with security groups</span></span>

<span data-ttu-id="5173d-103">**Pokud se zobrazí chyba sítě AADDS104**</span><span class="sxs-lookup"><span data-stu-id="5173d-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="5173d-104">Nejčastější příčinou chyb sítě pro Azure služba Active Directory Domain Services (služba AD DS) jsou neplatná pravidla skupiny zabezpečení služba AD DS.</span><span class="sxs-lookup"><span data-stu-id="5173d-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="5173d-105">Skupina zabezpečení sítě pro virtuální síť musí povolit přístup ke konkrétním portům a protokolům.</span><span class="sxs-lookup"><span data-stu-id="5173d-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="5173d-106">Pokud jsou tyto porty blokované, platforma Azure nemůže sledovat nebo aktualizovat spravovanou doménu.</span><span class="sxs-lookup"><span data-stu-id="5173d-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="5173d-107">Má vliv také synchronizace mezi Azure AD a služba AD DS Azure.</span><span class="sxs-lookup"><span data-stu-id="5173d-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="5173d-108">Zajistěte, abyste měli otevřené výchozí porty, abyste zabránili přerušení služby.</span><span class="sxs-lookup"><span data-stu-id="5173d-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="5173d-109">Informace o principech a řešení běžných upozornění týkajících se problémů s konfigurací skupiny zabezpečení sítě najdete v tématu [Přidání a ověření skupin zabezpečení.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)</span><span class="sxs-lookup"><span data-stu-id="5173d-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
