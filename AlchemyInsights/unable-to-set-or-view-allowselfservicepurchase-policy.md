---
title: Nelze nastavit nebo zobrazit zásady AllowSelfServicePurchase.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735192"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="21a8e-102">Nelze nastavit nebo zobrazit zásady AllowSelfServicePurchase.</span><span class="sxs-lookup"><span data-stu-id="21a8e-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="21a8e-103">Při pokusu o nastavení nebo zobrazení zásad AllowSelfServicePurchase se zobrazí tato chybová zpráva:</span><span class="sxs-lookup"><span data-stu-id="21a8e-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="21a8e-104">*HandleError: nepovedlo se načíst zásadu produktu s PolicyId AllowSelfServicePurchase, ErrorMessage – nadřízené připojení se zavřelo: došlo k neočekávané chybě při odeslání.*</span><span class="sxs-lookup"><span data-stu-id="21a8e-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="21a8e-105">Příčinou mohou být starší verze protokolu TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="21a8e-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="21a8e-106">Abyste mohli připojit službu MSCommerce, musíte používat TLS 1,2 nebo vyšší.</span><span class="sxs-lookup"><span data-stu-id="21a8e-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="21a8e-107">Zkuste použít následující postup pro povolení/nastavení protokolu TLS na 1,2, ověřte a zkuste to znova.</span><span class="sxs-lookup"><span data-stu-id="21a8e-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="21a8e-108">Na příkazovém řádku PowerShellu (PS C: \) Zadejte následující příkaz pro nastavení protokolu TLS na verzi 1,2:</span><span class="sxs-lookup"><span data-stu-id="21a8e-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="21a8e-109">Ověřte používané protokoly TLS pomocí následujícího příkazu:</span><span class="sxs-lookup"><span data-stu-id="21a8e-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="21a8e-110">Opakujte pokus o spuštění nebo aktualizaci podle potřeby.</span><span class="sxs-lookup"><span data-stu-id="21a8e-110">Retry the Get or Update commands as needed.</span></span>

