---
title: Diagnostika pro povolení základního ověřování Exchange Online protokolů
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11392"
- "9006699"
ms.openlocfilehash: 8952aba3dc6b5abcf56776d81eddd9b50db33c7f
ms.sourcegitcommit: d3a739b75d521837660ce151190a7e232e4eeadb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731301"
---
# <a name="diagnostic-to-enable-basic-authentication-for-exchange-online-protocols"></a><span data-ttu-id="d5ea0-102">Diagnostika pro povolení základního ověřování Exchange Online protokolů</span><span class="sxs-lookup"><span data-stu-id="d5ea0-102">Diagnostic to enable Basic authentication for Exchange Online protocols</span></span>

<span data-ttu-id="d5ea0-103">Pomocí této diagnostiky můžete povolit základní ověřování pro protokoly Exchange Online, jako jsou protokoly POP3, IMAP4, protokol Exchange ActiveSync, Exchange Web Services, Offline adresář, MAPI, RPC a Vzdálený PowerShell, které microsoft nedávno zakázal pro vaši organizaci.</span><span class="sxs-lookup"><span data-stu-id="d5ea0-103">By using this diagnostic, you can enable Basic authentication for Exchange Online protocols such as POP3, IMAP4, Exchange ActiveSync, Exchange Web Services, Offline Address Book, MAPI, RPC and Remote PowerShell, which Microsoft might have disabled recently for your organization.</span></span> 

<span data-ttu-id="d5ea0-104">Prostřednictvím Centra zpráv posíláme přímou komunikaci, aby tenantům věděli, kde jsou připravení vypnout základní ověřování ve svém prostředí z důvodu bez použití, což pomůže chránit jejich prostředí před souvisejícími bezpečnostními riziky.</span><span class="sxs-lookup"><span data-stu-id="d5ea0-104">We are sending direct communications through Message Center to let tenants know where they're ready to turn off Basic authentication in their environment due to no use, which will help protect their environments from related security risks.</span></span>