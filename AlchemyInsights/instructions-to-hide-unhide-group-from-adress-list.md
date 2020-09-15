---
title: Pokyny pro skrytí nebo zobrazení skupiny ze seznamu adres
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
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663002"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="a88ea-102">Skrytí skupiny Microsoft 365 ze seznamu adres (globální)</span><span class="sxs-lookup"><span data-stu-id="a88ea-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="a88ea-103">Pokud chcete skrýt skupinu Microsoft 365 ze seznamů adres klientů Exchange (jako je Outlook nebo OWA), použijte na EXO Shell tento příkaz:</span><span class="sxs-lookup"><span data-stu-id="a88ea-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="a88ea-104">Pokud chcete skupinu Microsoft 365 skrýt pro klienty Exchange, použijte následující příkaz v prostředí EXO:</span><span class="sxs-lookup"><span data-stu-id="a88ea-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

