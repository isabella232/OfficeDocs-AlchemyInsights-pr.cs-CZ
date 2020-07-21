---
title: Uživatel obdrží chybu AADSTS7000112 Yammer je zakázán
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197793"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="af519-102">Uživatel obdrží chybu AADSTS7000112 Yammer je zakázán</span><span class="sxs-lookup"><span data-stu-id="af519-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="af519-103">Pokud se zobrazí chyba "AADSTS7000112: Aplikace '0000005-0000-0ff1-ce00-0000000000000'(Yammer) je zakázáno,, existuje problém s hlavním školitým v rámci služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="af519-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="af519-104">Správce pravděpodobně zakázal objekt poskytování služeb, aby zablokoval přístup k Yammeru.</span><span class="sxs-lookup"><span data-stu-id="af519-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="af519-105">Zakázání objektu služby se nedoporučuje a může způsobit další problémy.</span><span class="sxs-lookup"><span data-stu-id="af519-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="af519-106">Další informace o podporovaném přístupu k blokování přístupu uživatelů k Yammeru najdete v tématu [Vypnutí přístupu Yammeru pro uživatele Microsoftu 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="af519-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="af519-107">Chcete-li tento problém opravit na webu Azure Portal a obnovit uživatelský přístup k Yammeru:</span><span class="sxs-lookup"><span data-stu-id="af519-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="af519-108">Otevřete stránku Služby Active Directory Azure a v levém navigačním podokně vyberte **Možnost Spravovat** **podnikové aplikace.**</span><span class="sxs-lookup"><span data-stu-id="af519-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="af519-109">Do vyhledávacího pole zadejte **Office 365 Yammer** a vyberte název aplikace, abyste otevřeli nastavení.</span><span class="sxs-lookup"><span data-stu-id="af519-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="af519-110">V levém navigačním podokně vyberte **Vlastnosti** v části **Spravovat.**</span><span class="sxs-lookup"><span data-stu-id="af519-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="af519-111">Nastavte hodnotu **Povoleno pro uživatele pro přihlášení?** na **Ano**a pak vyberte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="af519-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="af519-112">Znovu se přihlaste k Yammeru.</span><span class="sxs-lookup"><span data-stu-id="af519-112">Sign in to Yammer again.</span></span> <span data-ttu-id="af519-113">Možná budete muset vymazat soubory cookie.</span><span class="sxs-lookup"><span data-stu-id="af519-113">You might need to clear cookies.</span></span>

<span data-ttu-id="af519-114">Případně spusťte příkazy prostředí PowerShell a nastavte hodnotu.</span><span class="sxs-lookup"><span data-stu-id="af519-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="af519-115">Další informace najdete [v tématu "Omlouváme se, ale máme potíže s přihlášením" při kliknutí na dlaždici Yammeru v Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="af519-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 