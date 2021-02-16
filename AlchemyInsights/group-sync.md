---
title: Synchronizace skupin
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256684"
---
# <a name="group-sync"></a><span data-ttu-id="f45ff-102">Synchronizace skupin</span><span class="sxs-lookup"><span data-stu-id="f45ff-102">Group sync</span></span>

<span data-ttu-id="f45ff-103">Tento článek obsahuje pokyny k synchronizaci skupin.</span><span class="sxs-lookup"><span data-stu-id="f45ff-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="f45ff-104">Pokud globální správce nebo vlastník skupiny nemůže upravovat vlastnosti skupiny nebo přidávat členy nebo přiřazovat vlastníky na portálu Azure Portal, ujistěte se, že zdrojem autority pro skupinu je Azure Active Directory (Azure AD), který může globálnímu správci nebo vlastníkovi skupiny upravit skupinu.</span><span class="sxs-lookup"><span data-stu-id="f45ff-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="f45ff-105">Než se pokusíte odstranit synchronizované skupiny v [](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) Azure AD, ujistěte se, že jste odstranili všechny přiřazené licence, abyste se vyhnuli chybám.</span><span class="sxs-lookup"><span data-stu-id="f45ff-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="f45ff-106">Pokud chcete porozumět tomu, jak synchronizovat uživatele, skupiny a kontakty, podívejte se na Azure [AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)a sledujte synchronizaci místní skupiny s Azure pomocí Azure AD [Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) k synchronizaci místních skupin pomocí ad connect.</span><span class="sxs-lookup"><span data-stu-id="f45ff-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="f45ff-107">Postupujte podle této [příručky k řešení chyb při synchronizaci, které](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) vám pomohou vyřešit běžné chyby během synchronizace.</span><span class="sxs-lookup"><span data-stu-id="f45ff-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

