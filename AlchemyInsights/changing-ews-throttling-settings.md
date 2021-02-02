---
title: Změna nastavení omezení EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075890"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="c8dba-102">Změna nastavení omezení EWS</span><span class="sxs-lookup"><span data-stu-id="c8dba-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="c8dba-103">Spusťte prosím náš automatizovaný test, který vám umožní upravit zásady omezení EWS po dobu trvání migrace.</span><span class="sxs-lookup"><span data-stu-id="c8dba-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="c8dba-104">Upozorňujeme, že i po tomto spuštění budou importy EWS stále omezeny na 150 MB za 5 minut na poštovní schránku. Pokud chcete dosáhnout vyšší propustnosti migrace, migrujte prosím více uživatelů současně.</span><span class="sxs-lookup"><span data-stu-id="c8dba-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="c8dba-105">Nezapomeňte prosím, že změny zásad omezení EWS nemají žádný vliv na následující typy migrace (pomocí nástrojů Microsoftu): hybridní, přímou nebo fází (RPC/HTTP), IMAP, sadu G Suite, veřejnou složku nebo službu importu PST.</span><span class="sxs-lookup"><span data-stu-id="c8dba-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>