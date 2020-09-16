---
title: O identitě v Yammeru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664163"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="d00f4-102">O identitě v Yammeru</span><span class="sxs-lookup"><span data-stu-id="d00f4-102">About identity in Yammer</span></span>

<span data-ttu-id="d00f4-103">Doporučujeme, aby všechny sítě vybraly následující kroky, aby nedošlo k problémům s identitou:</span><span class="sxs-lookup"><span data-stu-id="d00f4-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="d00f4-104">Po zřízení účtů Microsoft 365 pro uživatele v Azure AD vynuťte identitu Office 365, aby se všichni uživatelé přihlásili pomocí svého primárního účtu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d00f4-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="d00f4-105">Další informace najdete v článku [vynucení identity Office 365 pro uživatele Yammeru](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="d00f4-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="d00f4-106">Konsolidujte více sítí Yammer.</span><span class="sxs-lookup"><span data-stu-id="d00f4-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="d00f4-107">Starší konfigurace Yammeru umožňují spojení více sítí Yammer s jedním nájemcem.</span><span class="sxs-lookup"><span data-stu-id="d00f4-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="d00f4-108">Další informace najdete v tématu [migrace sítě – sloučení více sítí Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="d00f4-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="d00f4-109">Volitelně můžete vynucením licencování pro Yammer blokovat uživatele z Yammeru, pokud nemají licenci.</span><span class="sxs-lookup"><span data-stu-id="d00f4-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="d00f4-110">Další informace najdete v článku [Správa uživatelských licencí Yammeru v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="d00f4-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="d00f4-111">Nakonec zkontrolujte seznam uživatelů pro starší sítě Yammer a pozastavte starší uživatele.</span><span class="sxs-lookup"><span data-stu-id="d00f4-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="d00f4-112">Doporučujeme, abyste uživatelé přezastavili (deaktivoval), protože odstranění je nevratné.</span><span class="sxs-lookup"><span data-stu-id="d00f4-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="d00f4-113">Další informace najdete v článku [auditování uživatelů Yammeru v sítích připojených k Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) a [odebrání uživatelů](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="d00f4-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="d00f4-114">Konfigurací Yammeru pomocí těchto kroků budete moct taky nakonfigurovat svou síť Yammer pro nativní režim pro Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d00f4-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="d00f4-115">Další informace najdete v článku [Konfigurace sítě Yammer pro nativní režim pro Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="d00f4-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>