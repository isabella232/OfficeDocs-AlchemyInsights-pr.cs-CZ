---
title: Poradce při potížích s vlastníkem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900794"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="9d473-102">Poradce při potížích s vlastníkem</span><span class="sxs-lookup"><span data-stu-id="9d473-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="9d473-103">Pokud chcete vyřešit problémy související s vlastníkem, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="9d473-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="9d473-104">[Přidání nebo změna správců předplatného Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): skupiny Azure Active Directory (Azure AD) jsou vlastněny a spravovány vlastníky skupiny.</span><span class="sxs-lookup"><span data-stu-id="9d473-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="9d473-105">Vlastníci skupiny můžou být uživatelé nebo hlavní objekty a můžou spravovat skupinu včetně členství.</span><span class="sxs-lookup"><span data-stu-id="9d473-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="9d473-106">Vlastníci skupiny můžou přiřadit jenom stávající vlastníci skupiny nebo správci skupiny.</span><span class="sxs-lookup"><span data-stu-id="9d473-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="9d473-107">Vlastníkům skupin není potřeba být členy skupiny.</span><span class="sxs-lookup"><span data-stu-id="9d473-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="9d473-108">[Přidání nebo změna správců předplatného Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): Tento článek popisuje, jak přidat nebo změnit roli správce pro uživatele v Azure RBAC v oboru předplatného.</span><span class="sxs-lookup"><span data-stu-id="9d473-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="9d473-109">K přidání vlastníka skupiny nebo vlastníka aplikace použijte PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9d473-109">Use PowerShell to add a group owner or an application owner.</span></span>
