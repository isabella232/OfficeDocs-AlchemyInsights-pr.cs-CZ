---
title: Nelze nastavit nebo zobrazit zásadu AllowSelfServicePurchase.
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826084"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="4158b-102">Nelze nastavit nebo zobrazit zásadu AllowSelfServicePurchase.</span><span class="sxs-lookup"><span data-stu-id="4158b-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="4158b-103">Při pokusu o nastavení nebo zobrazení zásad AllowSelfServicePurchase se zobrazí následující chybová zpráva:</span><span class="sxs-lookup"><span data-stu-id="4158b-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="4158b-104">*Chyba_zpracování: Nepodařilo se načíst zásady produktu pomocí id_zásady AllowSelfServicePurchase, ErrorMessage – základní připojení bylo uzavřeno: Při odeslání došlo k neočekávané chybě.*</span><span class="sxs-lookup"><span data-stu-id="4158b-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="4158b-105">Může to být způsobeno starší verzí tls (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="4158b-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="4158b-106">Pokud chcete připojit službu MSCommerce, musíte použít TLS 1.2 nebo vyšší.</span><span class="sxs-lookup"><span data-stu-id="4158b-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="4158b-107">Zkuste protokol TLS povolit nebo nastavit na 1.2, ověřit ho a zkusit to znovu.</span><span class="sxs-lookup"><span data-stu-id="4158b-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="4158b-108">Na příkazovém řádku PowerShellu (PS C: zadejte následující příkaz, který nastaví protokol \) TLS na verzi 1.2:</span><span class="sxs-lookup"><span data-stu-id="4158b-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="4158b-109">Ověřte používaný protokol TLS pomocí následujícího příkazu:</span><span class="sxs-lookup"><span data-stu-id="4158b-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="4158b-110">Podle potřeby opakujte příkazy Získat nebo Aktualizovat.</span><span class="sxs-lookup"><span data-stu-id="4158b-110">Retry the Get or Update commands as needed.</span></span>

