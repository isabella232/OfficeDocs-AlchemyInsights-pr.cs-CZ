---
title: Poradce při potížích s kódem chyby AADSTS50011
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9802"
- "9005744"
ms.openlocfilehash: 6acf0ce3615669babd1a912ffd782b3750b93500
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035708"
---
# <a name="troubleshoot-error-code-aadsts50011"></a><span data-ttu-id="48d6a-102">Poradce při potížích s kódem chyby AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="48d6a-102">Troubleshoot error code AADSTS50011</span></span>

<span data-ttu-id="48d6a-103">Pokud chcete vyřešit chybu AADSTS50011, proveďte níže popsaný doporučený krok.</span><span class="sxs-lookup"><span data-stu-id="48d6a-103">To resolve AADSTS50011 error, perform the recommended step described below.</span></span>

<span data-ttu-id="48d6a-104">**AADSTS50011**: InvalidReplyTo – adresa odpovědi chybí, chybně nakonfigurovaná nebo neodpovídá adresám odpovědí nakonfigurovaných pro aplikaci.</span><span class="sxs-lookup"><span data-stu-id="48d6a-104">**AADSTS50011**: InvalidReplyTo - The reply address is missing, misconfigured, or does not match reply addresses configured for the app.</span></span>

<span data-ttu-id="48d6a-105">Jako řešení zajistěte, aby se tato chybějící adresa odpovědi přidala do aplikace Azure Active Directory (AD) nebo aby to udělal někdo s oprávněními ke správě vaší aplikace ve službě AD.</span><span class="sxs-lookup"><span data-stu-id="48d6a-105">As a resolution ensure to add this missing reply address to the Azure Active Directory (AD) app or have someone with the permissions to manage your application in AD do this for you.</span></span> <span data-ttu-id="48d6a-106">Další informace najdete v článku o řešení potíží s [chybou AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch).</span><span class="sxs-lookup"><span data-stu-id="48d6a-106">For more information, see the troubleshooting article for error [AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch).</span></span>