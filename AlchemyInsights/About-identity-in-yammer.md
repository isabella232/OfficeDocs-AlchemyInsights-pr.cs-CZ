---
title: O identitě v Yammeru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148199"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="3ac94-102">O identitě v Yammeru</span><span class="sxs-lookup"><span data-stu-id="3ac94-102">About identity in Yammer</span></span>

<span data-ttu-id="3ac94-103">Doporučuje se, aby všechny sítě provést následující kroky, aby se zabránilo problémy související s identitou:</span><span class="sxs-lookup"><span data-stu-id="3ac94-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="3ac94-104">Vynuťte identitu Office 365 po zřizování účtů Microsoft 365 pro uživatele ve službě Azure AD, abyste zajistili, že se všichni uživatelé přihlásí pomocí svého primárního účtu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3ac94-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="3ac94-105">Další informace najdete v [tématu Vynucení identity Office 365 pro uživatele Yammeru](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="3ac94-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="3ac94-106">Konsolidujte více sítí Yammer.</span><span class="sxs-lookup"><span data-stu-id="3ac94-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="3ac94-107">Starší konfigurace Yammeru umožňují připojení více sítí Yammeru k jednomu klientovi.</span><span class="sxs-lookup"><span data-stu-id="3ac94-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="3ac94-108">Další informace najdete v [tématu Migrace v síti – konsolidace více sítí Yammeru](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="3ac94-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="3ac94-109">Volitelně můžete vynutit licencování pro Yammer, aby uživatelé z Yammeru zablokovali, pokud nemají licenci.</span><span class="sxs-lookup"><span data-stu-id="3ac94-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="3ac94-110">Další informace najdete [v tématu Správa uživatelských licencí Yammeru v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="3ac94-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="3ac94-111">Nakonec auditovat seznam uživatelů pro starší sítě Yammer a pozastavit starší uživatele.</span><span class="sxs-lookup"><span data-stu-id="3ac94-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="3ac94-112">Doporučujeme uživatele pozastavit (deaktivovat) namísto jejich odstranění, protože odstranění je nevratné.</span><span class="sxs-lookup"><span data-stu-id="3ac94-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="3ac94-113">Další informace najdete v [tématech Auditování uživatelů Yammeru v sítích připojených k Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) a [Odebrání uživatelů](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="3ac94-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="3ac94-114">Pokud yammer nakonfigurujete pomocí těchto kroků, budete taky připraveni nakonfigurovat síť Yammeru pro nativní režim pro Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3ac94-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="3ac94-115">Další informace najdete v [tématu Konfigurace sítě Yammer pro nativní režim pro Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="3ac94-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>