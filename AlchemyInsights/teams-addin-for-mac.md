---
title: Teams pro Mac
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
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582063"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="8031d-102">Teams pro Mac</span><span class="sxs-lookup"><span data-stu-id="8031d-102">Teams add-in for Mac</span></span>

<span data-ttu-id="8031d-103">Pokud chcete vyřešit Teams pro uživatele operačního systému Mac, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="8031d-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="8031d-104">**Krok 1:** Pokud máte místní hybridní Exchange (2016 CU3 nebo novější), ověřte pomocí nástroje Test-HMA.ps1, že je hybridní moderní ověřování správně nakonfigurované.</span><span class="sxs-lookup"><span data-stu-id="8031d-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="8031d-105">Další informace najdete v tématu Ověření nastavení hybridního moderního ověřování pro [Outlook pro iOS](https://aka.ms/TestHMAEAS)a Android.</span><span class="sxs-lookup"><span data-stu-id="8031d-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="8031d-106">**Poznámka:** Použijte formát adresy hlavní název uživatele (například [username@contoso.com](mailto:username@contoso.com)), ne doménu\uživatelské_jméno.</span><span class="sxs-lookup"><span data-stu-id="8031d-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="8031d-107">To můžete udělat i pro uživatele s Exchange Online poštovními schránkami.</span><span class="sxs-lookup"><span data-stu-id="8031d-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="8031d-108">**Krok 2:** Have the user go to **Tools**  >  **Accounts**... v Outlook pro Mac a vyhledejte a vyberte účet.</span><span class="sxs-lookup"><span data-stu-id="8031d-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="8031d-109">Potvrďte, že uvedené uživatelské jméno je ve formátu hlavní název uživatele (například [username@contoso.com).](mailto:username@contoso.com)</span><span class="sxs-lookup"><span data-stu-id="8031d-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="8031d-110">**Krok 3:** Potvrďte, že uživatel je licencovaný Microsoft Teams uživatele.</span><span class="sxs-lookup"><span data-stu-id="8031d-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="8031d-111">Uživatel musí používat předplatné Office 365 for Mac, produkt verze 16.24 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="8031d-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>