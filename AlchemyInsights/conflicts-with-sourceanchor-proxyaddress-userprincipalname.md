---
title: Konflikty s SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 877c954bea219cf8d885645cd25e41a5b7bab6fd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713447"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="03b76-102">Konflikty s SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="03b76-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="03b76-103">Pokud během synchronizace dojde k chybám, jako je například synchronizovaný objekt se stejnou ProxyAddress nebo UserPrincipalName ve vašem adresáři, přečtěte si článek [Diagnostika a náprava chyb synchronizace duplicitních atributů](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="03b76-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="03b76-104">Zvažte také možnost povolit odolnost duplicitních atributů.</span><span class="sxs-lookup"><span data-stu-id="03b76-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="03b76-105">Další informace najdete v tématu [synchronizace identit a odolnost duplicitních atributů](https://aka.ms/duplicateattributeresiliency).</span><span class="sxs-lookup"><span data-stu-id="03b76-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>