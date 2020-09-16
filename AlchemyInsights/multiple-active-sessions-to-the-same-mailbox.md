---
title: Vícenásobné aktivní relace do stejné poštovní schránky
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: f4ae5c5afef9972ad4ffe74144d702ed58b2f437
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769716"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="05535-102">Vícenásobné aktivní relace do stejné poštovní schránky</span><span class="sxs-lookup"><span data-stu-id="05535-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="05535-103">Za účelem řízení využití prostředků Exchange má poštovní schránka "rozpočet".</span><span class="sxs-lookup"><span data-stu-id="05535-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="05535-104">Výjimku z více rozpočtů lze aktivovat, ale není omezena na tyto okolnosti:</span><span class="sxs-lookup"><span data-stu-id="05535-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="05535-105">Ve stejné relaci Outlook Web Appu se otevírají několik karet prohlížeče.</span><span class="sxs-lookup"><span data-stu-id="05535-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="05535-106">Několik aktivních relací Outlook Web Appu ke stejné poštovní schránce.</span><span class="sxs-lookup"><span data-stu-id="05535-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="05535-107">Několik dalších klientských aplikací (Outlook, Outlook Mobile, klientská aplikace třetí strany) k poštovní schránce přistupuje současně.</span><span class="sxs-lookup"><span data-stu-id="05535-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="05535-108">Operace s dlouhým provozem, třeba provádění požadavků hledání, se provádějí z jiné aktivní relace poštovní schránky.</span><span class="sxs-lookup"><span data-stu-id="05535-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

