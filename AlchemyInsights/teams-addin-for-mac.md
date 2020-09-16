---
title: Doplněk Teams pro Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670321"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="13ad7-102">Doplněk Teams pro Mac</span><span class="sxs-lookup"><span data-stu-id="13ad7-102">Teams add-in for Mac</span></span>

<span data-ttu-id="13ad7-103">Pokud chcete vyřešit problém s chybějícím doplňkem Teams pro Mac, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="13ad7-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="13ad7-104">**Krok 1:** Pokud máte hybridní místní Exchange Server (2016 CU3 nebo novější), pomocí nástroje Test-HMA.ps1 potvrďte, že je hybridní moderní ověřování správně nakonfigurované.</span><span class="sxs-lookup"><span data-stu-id="13ad7-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="13ad7-105">Další informace najdete v článku [ověření nastavení hybridního moderního ověřování pro Outlook pro iOS a Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="13ad7-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="13ad7-106">**Poznámka:** Používejte formát adresy UPN (například [username@contoso.com](mailto:username@contoso.com)), ne doména \ uživatelské_jméno.</span><span class="sxs-lookup"><span data-stu-id="13ad7-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="13ad7-107">Používejte to i pro uživatele s poštovními schránkami Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="13ad7-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="13ad7-108">**Krok 2:** Přejděte na **Tools**  >  **účty**nástrojů... v Outlooku pro Mac a najděte a vyberte účet.</span><span class="sxs-lookup"><span data-stu-id="13ad7-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="13ad7-109">Potvrďte, že uvedené uživatelské jméno je ve formátu UPN (například [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="13ad7-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="13ad7-110">**Krok 3:** Ověřte, jestli je uživatel licencovaným uživatelem Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="13ad7-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="13ad7-111">Uživatel musí používat předplatné Office 365 for Mac, verzi produktu 16,24 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="13ad7-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>