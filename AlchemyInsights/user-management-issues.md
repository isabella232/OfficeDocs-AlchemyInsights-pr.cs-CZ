---
title: Problémy se s řízením uživatelů
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
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035138"
---
# <a name="user-management-issues"></a><span data-ttu-id="7891d-102">Problémy se s řízením uživatelů</span><span class="sxs-lookup"><span data-stu-id="7891d-102">User management issues</span></span>

<span data-ttu-id="7891d-103">**Co se stane s aktuálními přiřazenými uživateli aplikace, když zakážem vlastnost "Přiřazení uživatele je povinné" (tato vlastnost se nastaví na Ne)?**</span><span class="sxs-lookup"><span data-stu-id="7891d-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="7891d-104">Zakázání **povinného přiřazení uživatele** nemá vliv na aktuálně přiřazené uživatele.</span><span class="sxs-lookup"><span data-stu-id="7891d-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="7891d-105">Zakázání této vlastnosti umožní přístup k aplikaci jenom všem uživatelům.</span><span class="sxs-lookup"><span data-stu-id="7891d-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="7891d-106">Všichni uvedená uživatelé a uživatelé přiřazení ke skupinám v aplikaci budou i nadále platní.</span><span class="sxs-lookup"><span data-stu-id="7891d-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="7891d-107">Pokud chcete aplikaci omezit na konkrétní sadu uživatelů, podívejte se na článek – Omezení aplikace Azure AD na sadu uživatelů [– platforma identit Microsoftu | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span><span class="sxs-lookup"><span data-stu-id="7891d-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="7891d-108">Pokud chcete přiřazovat uživatele a skupiny, k podnikovým aplikacím v Azure Active Directory (Azure AD), ať už z webu Azure Portal, nebo pomocí PowerShellu, podívejte se na tématu Správa přiřazení uživatelů pro aplikaci v [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span><span class="sxs-lookup"><span data-stu-id="7891d-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="7891d-109">Pokud chcete delegovat oprávnění k vytváření a správě aplikací, podívejte se na delegování oprávnění správce správy [aplikací – Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span><span class="sxs-lookup"><span data-stu-id="7891d-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="7891d-110">**Skrytí konkrétních podnikových aplikací** uživatelům : Pomocí následujících kroků skryjte všechny aplikace Microsoft 365 z panelu **MyApps.**</span><span class="sxs-lookup"><span data-stu-id="7891d-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="7891d-111">Aplikace budou pořád viditelné na portálu Office 365.</span><span class="sxs-lookup"><span data-stu-id="7891d-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="7891d-112">Přihlaste se k webu Azure Portal jako globální správce vašeho adresáře.</span><span class="sxs-lookup"><span data-stu-id="7891d-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="7891d-113">Vyberte **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="7891d-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="7891d-114">Vyberte **Uživatelé**.</span><span class="sxs-lookup"><span data-stu-id="7891d-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="7891d-115">Vyberte **Nastavení uživatele**.</span><span class="sxs-lookup"><span data-stu-id="7891d-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="7891d-116">V **části Podnikové aplikace** klikněte na Spravovat způsob spouštění a prohlížení aplikací **koncovým uživatelům.**</span><span class="sxs-lookup"><span data-stu-id="7891d-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="7891d-117">Uživatelé **uvidí jenom aplikace Office 365 na portálu Office 365** a kliknou na **Ano.**</span><span class="sxs-lookup"><span data-stu-id="7891d-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="7891d-118">Klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="7891d-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="7891d-119">Další podrobnosti najdete v tématu skrytí podnikové aplikace z uživatelského prostředí [v Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span><span class="sxs-lookup"><span data-stu-id="7891d-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="7891d-120">Pokud mnoha organizacím nabízíte aplikaci Software jako služba (SaaS), můžete aplikaci nakonfigurovat tak, aby přijímaly přihlášení z libovolného tenanta Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="7891d-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="7891d-121">Tato konfigurace se nazývá "vytvoření více tenantů vaší aplikace".</span><span class="sxs-lookup"><span data-stu-id="7891d-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="7891d-122">Uživatelé v libovolném tenantovi Azure AD se budou moct přihlásit k vaší aplikaci po souhlasu s používáním svého účtu s vaší aplikací.</span><span class="sxs-lookup"><span data-stu-id="7891d-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="7891d-123">Další informace najdete v tématu [Vytváření aplikací, které se přihlaší k uživatelům Azure AD – platforma identit Microsoftu | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span><span class="sxs-lookup"><span data-stu-id="7891d-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="7891d-124">**Jak může koncový uživatel získat přístup k aplikaci, jakmile je k aplikaci přiřazen?**</span><span class="sxs-lookup"><span data-stu-id="7891d-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="7891d-125">Každá aplikace v okně aplikace Enterprise má odkaz pro přístup koncových uživatelů.</span><span class="sxs-lookup"><span data-stu-id="7891d-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="7891d-126">Uživatelé mají k aplikaci snadný přístup také prostřednictvím portálu **Myapps.**</span><span class="sxs-lookup"><span data-stu-id="7891d-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="7891d-127">**Chcete vědět, které aplikace a typy aplikací používají uživatelé?**</span><span class="sxs-lookup"><span data-stu-id="7891d-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="7891d-128">Sestavy přihlášení za posledních 30 dní si můžete stáhnout z portal.azure.com > **Azure Active directory> Signins> stáhnout sestavy.**</span><span class="sxs-lookup"><span data-stu-id="7891d-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="7891d-129">Zjistěte, jak udělit souhlas [správce celého tenanta](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) s aplikací a Konfigurace souhlasu [koncových uživatelů s aplikacemi](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span><span class="sxs-lookup"><span data-stu-id="7891d-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="7891d-130">[Pochopte, jak souhlas funguje,](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) [a Správa souhlasu s aplikacemi](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span><span class="sxs-lookup"><span data-stu-id="7891d-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>


