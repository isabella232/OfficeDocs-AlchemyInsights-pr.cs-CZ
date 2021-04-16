---
title: Exchange PowerShell a zastaralé základní ověřování
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813465"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="32bd5-102">Exchange PowerShell a zastaralé základní ověřování</span><span class="sxs-lookup"><span data-stu-id="32bd5-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="32bd5-103">Nejnovější informace o tom, jak se připojit k PowerShellu pro Exchange Online bez použití základního ověřování, najdete [tady](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="32bd5-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="32bd5-104">Modul PowerShell V2 nepoužívá základní ověřování.</span><span class="sxs-lookup"><span data-stu-id="32bd5-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="32bd5-105">Mějte prosím na paměti, že základní ověřování musí být na klientském počítači nadále povolené.</span><span class="sxs-lookup"><span data-stu-id="32bd5-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="32bd5-106">Nový modul PowerShell V2 používá k navázání připojení u všech rutin V2 založených na rozhraní REST moderní ověřování.</span><span class="sxs-lookup"><span data-stu-id="32bd5-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="32bd5-107">Kromě rutin V2 vám také umožňuje přístup ke starším rutinám vzdáleného PowerShellu (RPS), které vyžadují navázání relace vzdáleného PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="32bd5-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="32bd5-108">Navázání relace RPS na počítači s Windows vyžaduje, aby bylo na klientském počítači povolené ověřování WinRM BasicAuth, i když modul k ověření služby používá mechanismus moderního ověřování.</span><span class="sxs-lookup"><span data-stu-id="32bd5-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="32bd5-109">K přenosu tokenů moderního ověřování se používá kanál základního ověřování WinRM.</span><span class="sxs-lookup"><span data-stu-id="32bd5-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="32bd5-110">Pokud je na klientském počítači základní ověřování WinRM zakázané, budou nové rutiny V2 dál fungovat (ale ne starší rutiny RPS).</span><span class="sxs-lookup"><span data-stu-id="32bd5-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
