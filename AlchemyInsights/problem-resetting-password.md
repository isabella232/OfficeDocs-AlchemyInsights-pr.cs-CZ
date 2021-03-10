---
title: Problém s resetováním hesla
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693392"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="44050-102">Problémy s resetováním hesla</span><span class="sxs-lookup"><span data-stu-id="44050-102">Problems resetting password</span></span>

<span data-ttu-id="44050-103">Tady jsou některé problémy, se které se můžou zobrazit při resetování hesla, a možná řešení:</span><span class="sxs-lookup"><span data-stu-id="44050-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="44050-104">**Mám problém s resetováním hesla, který není zahrnutý v ostatních kategoriích**</span><span class="sxs-lookup"><span data-stu-id="44050-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="44050-105">Ujistěte se, že máte oprávnění k resetování hesel.</span><span class="sxs-lookup"><span data-stu-id="44050-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="44050-106">Hesla uživatele můžou resetovat jenom globální správci a správci uživatelů.</span><span class="sxs-lookup"><span data-stu-id="44050-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="44050-107">Globální správci můžou taky resetovat hesla jiných privilegovaných správců.</span><span class="sxs-lookup"><span data-stu-id="44050-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="44050-108">Ujistěte se, že rozumíte licenčním požadavkům:</span><span class="sxs-lookup"><span data-stu-id="44050-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="44050-109">Ve vaší organizaci musíte mít přiřazenou aspoň jednu licenci.</span><span class="sxs-lookup"><span data-stu-id="44050-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="44050-110">Jenom cloudové uživatele – všechny placené SKU Office 365 (O365) nebo Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="44050-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="44050-111">Cloudové a místní uživatele – Azure AD Premium P1 nebo P2, Enterprise Mobility + Security (EMS) nebo Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="44050-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="44050-112">Další informace o licenčních požadavcích najdete v článku Licenční požadavky pro samoobslužné resetování [hesla Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="44050-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="44050-113">**Mám problémy s testováním nastavené zásady resetování hesla**</span><span class="sxs-lookup"><span data-stu-id="44050-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="44050-114">Může trvat několik minut, než se použité zásady replikují do všech datových center a koncových bodů.</span><span class="sxs-lookup"><span data-stu-id="44050-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="44050-115">Na to, jak rychle se změny použijí, ovlivní taky fyzická vzdálenost od datového centra.</span><span class="sxs-lookup"><span data-stu-id="44050-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="44050-116">Testujte s koncovým uživatelem, ne s správcem, a pilotním testováním s malou sadu uživatelů.</span><span class="sxs-lookup"><span data-stu-id="44050-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="44050-117">Zásady nakonfigurované na portálu Azure Portal platí JENOM pro koncové uživatele, ne pro správce.</span><span class="sxs-lookup"><span data-stu-id="44050-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="44050-118">Microsoft vynucuje silné výchozí zásady resetování hesla ve dvou bránách pro libovolnou roli správce Azure (Příklad: Globální správce, Správce helpdesku, Správce hesel atd.)</span><span class="sxs-lookup"><span data-stu-id="44050-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="44050-119">Přečtěte si další [informace o zásadách pro správce.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="44050-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="44050-120">**Chci nasadit resetování hesla, ale nechci, aby uživatelé zaregistroval další bezpečnostní údaje**</span><span class="sxs-lookup"><span data-stu-id="44050-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="44050-121">Data uživatelů můžete předem vyplnit, takže je nemusíte vyplnit.</span><span class="sxs-lookup"><span data-stu-id="44050-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="44050-122">Jako správce můžete před zahájením resetování hesla pro vaši organizaci nastavit vlastnosti telefonu a e-mailu pro uživatele.</span><span class="sxs-lookup"><span data-stu-id="44050-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="44050-123">Můžete to udělat pomocí rozhraní API, PowerShellu nebo Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="44050-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="44050-124">Další informace najdete tady:</span><span class="sxs-lookup"><span data-stu-id="44050-124">More information here:</span></span>
- [<span data-ttu-id="44050-125">Nasazení resetování hesla bez nutnosti registrace uživatelů</span><span class="sxs-lookup"><span data-stu-id="44050-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="44050-126">Jaká data se používají při resetování hesla?</span><span class="sxs-lookup"><span data-stu-id="44050-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="44050-127">**Tlačítko pro resetování hesla se zobrazí šedě**</span><span class="sxs-lookup"><span data-stu-id="44050-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="44050-128">K resetování hesel tohoto uživatele nejste oprávněni.</span><span class="sxs-lookup"><span data-stu-id="44050-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="44050-129">Hesla uživatele můžou resetovat jenom globální správci a správci uživatelů.</span><span class="sxs-lookup"><span data-stu-id="44050-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="44050-130">Globální správci můžou taky resetovat hesla jiných privilegovaných správců.</span><span class="sxs-lookup"><span data-stu-id="44050-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="44050-131">**Nevidím list pro resetování hesla**</span><span class="sxs-lookup"><span data-stu-id="44050-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="44050-132">K resetování hesel máte oprávnění.</span><span class="sxs-lookup"><span data-stu-id="44050-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="44050-133">Hesla uživatele můžou resetovat jenom globální správci a správci uživatelů.</span><span class="sxs-lookup"><span data-stu-id="44050-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="44050-134">Globální správci můžou taky resetovat hesla jiných privilegovaných správců.</span><span class="sxs-lookup"><span data-stu-id="44050-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="44050-135">**Při resetování hesla nevidím místní integraci s listy**</span><span class="sxs-lookup"><span data-stu-id="44050-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="44050-136">Místní integrace se zobrazuje jenom v hybridních prostředích, což znamená, že používáte k práci s hesly místních uživatelů zpětný zápis hesel.</span><span class="sxs-lookup"><span data-stu-id="44050-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="44050-137">Tento list se nezekoumá, pokud:</span><span class="sxs-lookup"><span data-stu-id="44050-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="44050-138">Používáte bez zpětného zápisu hesla</span><span class="sxs-lookup"><span data-stu-id="44050-138">You are not using password writeback</span></span>
    - <span data-ttu-id="44050-139">Došlo k problému s instalací nebo připojením zpětného zápisu hesla</span><span class="sxs-lookup"><span data-stu-id="44050-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="44050-140">Došlo k problému s instalací nebo připojením služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="44050-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="44050-141">Další kroky pro řešení problémů s zpětným zápisem hesla najdete v části Řešení potíží [se zápisem hesla.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="44050-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="44050-142">**Nevím, jak resetovat heslo uživatele**</span><span class="sxs-lookup"><span data-stu-id="44050-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="44050-143">Přihlaste se k portálu Azure Portal jako příslušný správce.</span><span class="sxs-lookup"><span data-stu-id="44050-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="44050-144">Přejděte do okna Uživatelé a skupiny a vyberte **Všichni uživatelé.**</span><span class="sxs-lookup"><span data-stu-id="44050-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="44050-145">Vyberte uživatele ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="44050-145">Select a user from the list.</span></span>
1. <span data-ttu-id="44050-146">Pro vybraného uživatele vyberte **Přehled** a potom na panelu příkazů klikněte na **Resetovat heslo.**</span><span class="sxs-lookup"><span data-stu-id="44050-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="44050-147">Postupujte podle pokynů na obrazovce.</span><span class="sxs-lookup"><span data-stu-id="44050-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="44050-148">Obnovení pouze prostřednictvím zpětného zápisu hesla pro podporu na portálu Azure Portal</span><span class="sxs-lookup"><span data-stu-id="44050-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="44050-149">**Resetování hesla místního uživatele z portálu pro správu Office 365 nebo mobilní aplikace Office 365, ale uživatel se pořád nemůže přihlásit**</span><span class="sxs-lookup"><span data-stu-id="44050-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="44050-150">Na tomto portálu se nepodporuje zpětný zápis hesel.</span><span class="sxs-lookup"><span data-stu-id="44050-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="44050-151">Resetování uživatelského hesla znovu na portálu Azure Portal – portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="44050-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

