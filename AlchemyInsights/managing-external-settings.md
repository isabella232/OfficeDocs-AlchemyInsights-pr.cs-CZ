---
title: Správa externích nastavení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294169"
---
# <a name="managing-external-settings"></a><span data-ttu-id="e12f7-102">Správa externích nastavení</span><span class="sxs-lookup"><span data-stu-id="e12f7-102">Managing External Settings</span></span>

<span data-ttu-id="e12f7-103">**Oznámení**</span><span class="sxs-lookup"><span data-stu-id="e12f7-103">**Announcement**</span></span>

- <span data-ttu-id="e12f7-104">Od 4. ledna 2021 se od Googlu ode dne 4. ledna [2021 odepíše podpora přihlášení WebView.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="e12f7-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="e12f7-105">Otestujte, jestli se na vaše aplikace vliv mají, a to podle pokynů Googlu pro testování kompatibility.</span><span class="sxs-lookup"><span data-stu-id="e12f7-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="e12f7-106">Při přihlašování uživatelů pomocí spotřebitelských účtů Google nezapomeňte použít webové zobrazení systému nebo prohlížeč systému.</span><span class="sxs-lookup"><span data-stu-id="e12f7-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="e12f7-107">**Správa nastavení pozvánek**</span><span class="sxs-lookup"><span data-stu-id="e12f7-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="e12f7-108">Potvrďte, že jste [nakonfigurovali nastavení externí spolupráce tak,](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) aby se příslušnými lidmi mohly posílat pozvánky.</span><span class="sxs-lookup"><span data-stu-id="e12f7-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="e12f7-109">**Správa přístupových oprávnění uživatelů hosta**</span><span class="sxs-lookup"><span data-stu-id="e12f7-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="e12f7-110">Globální správci mohou spravovat přístupová oprávnění hostů v adresáři prostřednictvím portálu Azure Portal nakonfigurováním oprávnění pro přístup hostů na stránce Nastavení externí spolupráce.</span><span class="sxs-lookup"><span data-stu-id="e12f7-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="e12f7-111">[Přečtěte si další informace o tomto nastavení.](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="e12f7-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="e12f7-112">Pokud chcete, aby vaši hosté měli přístup k aplikacím, jako je Teams nebo SharePoint, potvrďte, že jste je nakonfigurovali tak, aby přístup hostů povoloval.</span><span class="sxs-lookup"><span data-stu-id="e12f7-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="e12f7-113">Přečtěte si další informace [o nastavení teams](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) a [SharePointu.](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="e12f7-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="e12f7-114">**Konfigurace pozvánek:**</span><span class="sxs-lookup"><span data-stu-id="e12f7-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="e12f7-115">Povolte externí spolupráci S2B a spravujte, kdo může zvat hosty.</span><span class="sxs-lookup"><span data-stu-id="e12f7-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="e12f7-116">Povolit nebo blokovat pozvánky uživatelům z určitých organizací</span><span class="sxs-lookup"><span data-stu-id="e12f7-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="e12f7-117">**Konfigurace povolených zprostředkovatelů identity:**</span><span class="sxs-lookup"><span data-stu-id="e12f7-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="e12f7-118">Google Federation</span><span class="sxs-lookup"><span data-stu-id="e12f7-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="e12f7-119">Přímá federace</span><span class="sxs-lookup"><span data-stu-id="e12f7-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="e12f7-120">Ověření e-mailového hesla v jednom e-mailu</span><span class="sxs-lookup"><span data-stu-id="e12f7-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
