---
title: Změna nastavení omezení EWS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818029"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="6c3ef-102">Změna nastavení omezení EWS</span><span class="sxs-lookup"><span data-stu-id="6c3ef-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="6c3ef-103">Spusťte prosím náš automatizovaný test, který vám umožní upravit zásady omezení EWS po dobu trvání migrace.</span><span class="sxs-lookup"><span data-stu-id="6c3ef-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="6c3ef-104">Všimněte si, že i po tomto spuštění budou importy EWS omezeny na 150 MB za 5 minut na poštovní schránku. pokud chcete dosáhnout vyšší propustnosti migrace, migrujte prosím více uživatelů současně.</span><span class="sxs-lookup"><span data-stu-id="6c3ef-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="6c3ef-105">Upozorňujeme, že změny zásad omezení EWS nemají vliv na následující typy migrace (pomocí nástrojů Microsoftu): Hybridní, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Veřejná složka nebo Služba importu PST.</span><span class="sxs-lookup"><span data-stu-id="6c3ef-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>