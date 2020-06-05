---
title: Oprava aplikací Microsoft 365 Nemohl najít přidruženou zprávu o licencích office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580434"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="81201-102">Oprava zprávy Aplikace Microsoft 365 "Nelze najít přidružené licence office"</span><span class="sxs-lookup"><span data-stu-id="81201-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="81201-103">Pokud se zobrazí tato zpráva, vyzkoušejte následující postup:</span><span class="sxs-lookup"><span data-stu-id="81201-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="81201-104">Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, zda neblokují přístup k Internetu aplikacím Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="81201-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="81201-105">Viz [Microsoft 365 URL a rozsahy IP adres](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="81201-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="81201-106">Odeberte a [znovu přiřaďte licenci Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) pro postiženého uživatele.</span><span class="sxs-lookup"><span data-stu-id="81201-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="81201-107">Otevřete aplikaci Office a [odhlaste se od](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) všech existujících uživatelských účtů.</span><span class="sxs-lookup"><span data-stu-id="81201-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="81201-108">Přejděte na Nastavení systému Windows > **účty**  >  **e-mail & účtů**a odeberte všechny pracovní účty kromě ovlivněného účtu.</span><span class="sxs-lookup"><span data-stu-id="81201-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="81201-109">Přejděte na Nastavení systému Windows > **Accounts**  >  **účty Přístup k práci nebo škole**a odpojte všechny pracovní účty kromě ovlivněného účtu.</span><span class="sxs-lookup"><span data-stu-id="81201-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="81201-110">Resetujte stav aktivace Office.</span><span class="sxs-lookup"><span data-stu-id="81201-110">Reset the Office activation state.</span></span> <span data-ttu-id="81201-111">[Přečtěte si, jak](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="81201-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="81201-112">[Přihlaste se](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocí ovlivněného uživatelského účtu.</span><span class="sxs-lookup"><span data-stu-id="81201-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="81201-113">Další řešení potíží najdete [v tématu Chyby nelicencovaného produktu a aktivace v Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="81201-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>