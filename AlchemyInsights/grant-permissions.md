---
title: Udělit oprávnění
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900958"
---
# <a name="grant-permissions"></a><span data-ttu-id="de6f2-102">Udělit oprávnění</span><span class="sxs-lookup"><span data-stu-id="de6f2-102">Grant permissions</span></span>

1. <span data-ttu-id="de6f2-103">**Udělování souhlasu správce pro tenanta**: Přečtěte si článek o tom, [jak udělit oprávnění správcům na úrovni tenanta pro aplikaci](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) pro podrobné pokyny pro udělení souhlasu správce pro celou tenanta z Azure Portalu pomocí Azure AD PowerShellu nebo z samotné výzvy k souhlasu.</span><span class="sxs-lookup"><span data-stu-id="de6f2-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="de6f2-104">**Udělení souhlasu jménem konkrétního uživatele**: namísto souhlasu celé organizace může správce pomocí [rozhraní Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) také udělit souhlas s delegovanými oprávněními jménem jednoho uživatele.</span><span class="sxs-lookup"><span data-stu-id="de6f2-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="de6f2-105">Další informace najdete v článku o [získání přístupu v zastoupení uživatele](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="de6f2-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>