---
title: Problémy s přihlašovacími údaji
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063598"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="280f9-102">Problémy s přihlašovacími údaji</span><span class="sxs-lookup"><span data-stu-id="280f9-102">Issues with credentials</span></span>

<span data-ttu-id="280f9-103">Platforma identit Microsoft a tok přihlašovacích údajů klienta [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) popisují, jak programovat přímo proti toku přihlašovacích údajů klienta OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="280f9-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="280f9-104">**Jak můžu spravovat přihlašovací údaje aplikace pro heslo nebo certifikát?**</span><span class="sxs-lookup"><span data-stu-id="280f9-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="280f9-105">V Azure CLI můžete přihlašovací údaje [aplikace az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) použít k odstranění, vytvoření seznamu nebo resetování přihlašovacích údajů pro heslo aplikace nebo certifikát.</span><span class="sxs-lookup"><span data-stu-id="280f9-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="280f9-106">**Jak si uživatelé resetují hesla?**</span><span class="sxs-lookup"><span data-stu-id="280f9-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="280f9-107">Uživatelé se musí [před resetováním](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) hesel zaregistrovat k samoobslužné resetování hesla.</span><span class="sxs-lookup"><span data-stu-id="280f9-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="280f9-108">Jakmile se uživatel zaregistroval, může si podle pokynů v tomto článku resetovat heslo: resetovat si pracovní nebo [školní heslo.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="280f9-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="280f9-109">**Jak si uživatelé změní hesla?**</span><span class="sxs-lookup"><span data-stu-id="280f9-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="280f9-110">Uživatelé mohou při změně hesla postupovat podle pokynů v tomto článku: Jak [si změnit heslo.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="280f9-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="280f9-111">Mohou také [spravovat hesla aplikací pro dvoukroové ověření.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="280f9-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="280f9-112">**Při změně nebo resetování hesla se uživateli zobrazí chyba**</span><span class="sxs-lookup"><span data-stu-id="280f9-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="280f9-113">Tento odkaz poskytne informace o běžných problémech, které mohou nastat při pokusu uživatele o resetování hesla: Běžné problémy a [jejich řešení.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="280f9-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="280f9-114">**Mám problém s resetováním uživatelského hesla**</span><span class="sxs-lookup"><span data-stu-id="280f9-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="280f9-115">Ujistěte se, že máte oprávnění k resetování hesel.</span><span class="sxs-lookup"><span data-stu-id="280f9-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="280f9-116">*Hesla uživatele můžou resetovat jenom globální správci a správci uživatelů.*</span><span class="sxs-lookup"><span data-stu-id="280f9-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="280f9-117">Globální správci můžou taky resetovat hesla jiných privilegovaných správců.</span><span class="sxs-lookup"><span data-stu-id="280f9-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="280f9-118">Ujistěte se, že rozumíte licenčním požadavkům:</span><span class="sxs-lookup"><span data-stu-id="280f9-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="280f9-119">Ve vaší organizaci musíte mít přiřazenou aspoň jednu licenci:</span><span class="sxs-lookup"><span data-stu-id="280f9-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="280f9-120">**Jenom cloudové uživatele** – všechny placené SKU Office 365 (O365) nebo Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="280f9-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="280f9-121">**Cloudové a místní** uživatele – Azure AD Premium P1 nebo P2, Enterprise Mobility + Security (EMS) nebo Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="280f9-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="280f9-122">Další informace o licenčních požadavcích najdete v článku o licenčních požadavcích pro samoobslužné resetování [hesla Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="280f9-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="280f9-123">Pokud chcete resetovat heslo uživatele, najděte uživatele v Azure AD.</span><span class="sxs-lookup"><span data-stu-id="280f9-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="280f9-124">Pak v listu přehledu pro tohoto uživatele klikněte na tlačítko Resetovat heslo.</span><span class="sxs-lookup"><span data-stu-id="280f9-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="280f9-125">**Tlačítko pro resetování hesla se zobrazí šedě**</span><span class="sxs-lookup"><span data-stu-id="280f9-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="280f9-126">K resetování hesel **tohoto** uživatele nejste oprávněni.</span><span class="sxs-lookup"><span data-stu-id="280f9-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="280f9-127">*Hesla uživatele můžou resetovat jenom globální správci, hesla a správci uživatelů.*</span><span class="sxs-lookup"><span data-stu-id="280f9-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="280f9-128">Globální správci můžou taky resetovat hesla jiných privilegovaných správců.</span><span class="sxs-lookup"><span data-stu-id="280f9-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="280f9-129">**Nevidím list pro resetování hesla**</span><span class="sxs-lookup"><span data-stu-id="280f9-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="280f9-130">K resetování hesel máte oprávnění.</span><span class="sxs-lookup"><span data-stu-id="280f9-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="280f9-131">*Hesla uživatele můžou resetovat jenom globální správci, hesla a správci uživatelů.*</span><span class="sxs-lookup"><span data-stu-id="280f9-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="280f9-132">Globální správci můžou taky resetovat hesla jiných privilegovaných správců.</span><span class="sxs-lookup"><span data-stu-id="280f9-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="280f9-133">**Při resetování hesla nevidím místní integraci s listy**</span><span class="sxs-lookup"><span data-stu-id="280f9-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="280f9-134">Místní integrace se zobrazuje jenom v hybridních prostředích, což znamená, že používáte k práci s hesly místních uživatelů zpětný zápis hesel.</span><span class="sxs-lookup"><span data-stu-id="280f9-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="280f9-135">Tento list se nezkoumá, pokud:</span><span class="sxs-lookup"><span data-stu-id="280f9-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="280f9-136">Používáte bez zpětného zápisu hesla</span><span class="sxs-lookup"><span data-stu-id="280f9-136">You are not using password writeback</span></span>
  - <span data-ttu-id="280f9-137">Došlo k problému s instalací nebo připojením zpětného zápisu hesla</span><span class="sxs-lookup"><span data-stu-id="280f9-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="280f9-138">Došlo k problému s instalací nebo připojením služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="280f9-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="280f9-139">Další kroky pro řešení problémů s zpětným zápisem hesla najdete v článku [Řešení potíží se zpětným zápisem hesla](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="280f9-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="280f9-140">**Nevím, jak resetovat heslo uživatele**</span><span class="sxs-lookup"><span data-stu-id="280f9-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="280f9-141">Přihlaste se k portálu Azure Portal jako příslušný správce.</span><span class="sxs-lookup"><span data-stu-id="280f9-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="280f9-142">Přejděte do okna **Uživatelé a skupiny** a vyberte Všichni **uživatelé.**</span><span class="sxs-lookup"><span data-stu-id="280f9-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="280f9-143">Vyberte uživatele ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="280f9-143">Select a user from the list.</span></span>
4. <span data-ttu-id="280f9-144">U vybraného uživatele vyberte **Přehled a** potom na panelu příkazů vyberte **Resetovat heslo.**</span><span class="sxs-lookup"><span data-stu-id="280f9-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="280f9-145">Vyberte tlačítko **Resetovat** heslo a postupujte podle pokynů na obrazovce.</span><span class="sxs-lookup"><span data-stu-id="280f9-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="280f9-146">Obnovení pouze prostřednictvím **zpětného zápisu** hesla pro podporu na portálu Azure Portal</span><span class="sxs-lookup"><span data-stu-id="280f9-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="280f9-147">**Resetování hesla místního uživatele z portálu pro správu Office 365 nebo mobilní aplikace Office 365, ale uživatel se pořád nemůže přihlásit**</span><span class="sxs-lookup"><span data-stu-id="280f9-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="280f9-148">Na tomto portálu se nepodporuje zpětný zápis hesel.</span><span class="sxs-lookup"><span data-stu-id="280f9-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="280f9-149">Resetujte heslo uživatele znovu na portálu Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="280f9-149">Reset the user's password again in the Azure portal.</span></span>
