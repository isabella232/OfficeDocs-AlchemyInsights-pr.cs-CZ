---
title: Port Google Chrome Extensions na Microsoft Edge (chrom)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676995"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="bfd1a-102">Port Google Chrome Extensions na Microsoft Edge (chrom)</span><span class="sxs-lookup"><span data-stu-id="bfd1a-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="bfd1a-103">[Můžete snadno přeportovat rozšíření Google Chrome na Microsoft Edge (chrom)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="bfd1a-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="bfd1a-104">Ve většině případů jsou pro spuštění těchto přípon v Microsoft Edge pouze minimální změny.</span><span class="sxs-lookup"><span data-stu-id="bfd1a-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="bfd1a-105">Rozhraní API rozšíření a klíče manifestu podporované v Google Chrome jsou kódem kompatibilním s Microsoft Edgem.</span><span class="sxs-lookup"><span data-stu-id="bfd1a-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="bfd1a-106">Microsoft Edge ale nepodporuje rozšíření API Chrome. GCM, Chrome. identity. getaccounts, Chrome. identity. getAuthToken a Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="bfd1a-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>