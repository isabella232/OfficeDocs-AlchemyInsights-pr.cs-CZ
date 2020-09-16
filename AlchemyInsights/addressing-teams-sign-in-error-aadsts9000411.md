---
title: Chyba při přihlašování týmů pro adresování AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687031"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="42d63-102">Chyba při přihlašování týmů pro adresování AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="42d63-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="42d63-103">Při přihlášení k Microsoft Teams se může zobrazit chyba: Bohužel máme **problémy s přihlášením v AADSTS9000411: žádost nemá správný formát. Parametr "login_hint" je duplicitní.**</span><span class="sxs-lookup"><span data-stu-id="42d63-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="42d63-104">Pokud chcete tento problém vyřešit, zkontrolujte, jestli máte aktualizované klienty Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="42d63-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="42d63-105">Další informace o aktualizaci klienta najdete v článku [aktualizace Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="42d63-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="42d63-106">Pokud z nějakého důvodu nemůžete klienta aktualizovat, odhlášení klienta vymaže data z mezipaměti.</span><span class="sxs-lookup"><span data-stu-id="42d63-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="42d63-107">Pokud ale máte problémy i po odhlášení nebo přihlášení, zavřete aplikace teams a zrušte zaškrtnutí následujícího:</span><span class="sxs-lookup"><span data-stu-id="42d63-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="42d63-108">Ukončete aplikaci Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="42d63-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="42d63-109">Přejděte na:%AppData%\microsoft\teams a odstraňte všechny soubory.</span><span class="sxs-lookup"><span data-stu-id="42d63-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="42d63-110">Znovu spusťte aplikaci Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="42d63-110">Reopen Microsoft Teams.</span></span>
