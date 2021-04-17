---
title: 'Oprava aplikací Microsoft 365: Nenašli jsme přidruženou zprávu o licencích office.'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816481"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="bf513-102">Oprava zprávy o tom, že aplikace Microsoft 365 nejsou přidružené k licencím office</span><span class="sxs-lookup"><span data-stu-id="bf513-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="bf513-103">Pokud se vám tato zpráva zobrazí, zkuste toto:</span><span class="sxs-lookup"><span data-stu-id="bf513-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="bf513-104">Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, že neblokují přístup k internetu k aplikacím Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bf513-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="bf513-105">Viz Adresy URL a rozsahy IP adres [microsoftu 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="bf513-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="bf513-106">Odeberte [a znovu přijměte licenci Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) pro postiženého uživatele.</span><span class="sxs-lookup"><span data-stu-id="bf513-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="bf513-107">Otevřete aplikaci Office a [odhlásit se od](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) všech existujících uživatelských účtů.</span><span class="sxs-lookup"><span data-stu-id="bf513-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="bf513-108">Přejděte na Nastavení Windows > **Účty**  >  **e-& účty** a odeberte všechny pracovní účty kromě ovlivněného účtu.</span><span class="sxs-lookup"><span data-stu-id="bf513-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="bf513-109">Přejděte na Nastavení Systému Windows > **účty Access** v práci nebo ve škole a odpojte všechny pracovní účty kromě  >  ovlivněného účtu.</span><span class="sxs-lookup"><span data-stu-id="bf513-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="bf513-110">Resetujte stav aktivace Office.</span><span class="sxs-lookup"><span data-stu-id="bf513-110">Reset the Office activation state.</span></span> <span data-ttu-id="bf513-111">[Zjistěte, jak](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)na to.</span><span class="sxs-lookup"><span data-stu-id="bf513-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="bf513-112">[Přihlaste se](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocí ovlivněného uživatelského účtu.</span><span class="sxs-lookup"><span data-stu-id="bf513-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="bf513-113">Další řešení pro řešení potíží najdete v [článku Chyby nelicencovaných](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)produktů a aktivace v Office .</span><span class="sxs-lookup"><span data-stu-id="bf513-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>