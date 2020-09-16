---
title: Oprava aplikací Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747688"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="2e9b2-102">Oprava aplikací Microsoft 365 se zprávou nenašly se licence Office přidružené.</span><span class="sxs-lookup"><span data-stu-id="2e9b2-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="2e9b2-103">Pokud se zobrazí tato zpráva, zkuste toto:</span><span class="sxs-lookup"><span data-stu-id="2e9b2-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="2e9b2-104">Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, že nejsou blokovány internetové připojení k aplikacím Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2e9b2-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="2e9b2-105">Viz [adresy URL a rozsahy IP adres pro Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="2e9b2-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="2e9b2-106">Odeberte a [přiřaďte licenci Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) příslušnému uživateli.</span><span class="sxs-lookup"><span data-stu-id="2e9b2-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="2e9b2-107">Otevřete aplikaci Office a [odhlaste](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) se z existujících uživatelských účtů.</span><span class="sxs-lookup"><span data-stu-id="2e9b2-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="2e9b2-108">Přejděte na nastavení Windows > **účty**  >  **e-mailem &** a odeberte všechny pracovní účty kromě příslušného účtu.</span><span class="sxs-lookup"><span data-stu-id="2e9b2-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="2e9b2-109">Přejděte na nastavení Windows > **účty**  >  **k práci nebo škole**a odpojte všechny pracovní účty kromě příslušného účtu.</span><span class="sxs-lookup"><span data-stu-id="2e9b2-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="2e9b2-110">Resetujte stav aktivace Office.</span><span class="sxs-lookup"><span data-stu-id="2e9b2-110">Reset the Office activation state.</span></span> <span data-ttu-id="2e9b2-111">[Zjistěte, jak](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="2e9b2-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="2e9b2-112">[Přihlaste](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) se pomocí příslušného uživatelského účtu.</span><span class="sxs-lookup"><span data-stu-id="2e9b2-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="2e9b2-113">Další řešení pro řešení potíží najdete [v článku chyby typu nelicencovaný produkt a chyby aktivace v Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="2e9b2-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>