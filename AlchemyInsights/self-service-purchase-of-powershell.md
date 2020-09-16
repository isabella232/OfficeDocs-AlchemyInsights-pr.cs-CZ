---
title: Samoobslužný nákup PowerShellu
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
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739963"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="dcf87-102">Samoobslužný nákup PowerShellu</span><span class="sxs-lookup"><span data-stu-id="dcf87-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="dcf87-103">Pokud chcete používat modul PowerShell MSCommerce, musíte ho nainstalovat na zařízení s Windows 10 s TLS 1,2 (vyžaduje se oprávnění místního správce).</span><span class="sxs-lookup"><span data-stu-id="dcf87-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="dcf87-104">Importujte modul MSCommerce a připojte se k němu.</span><span class="sxs-lookup"><span data-stu-id="dcf87-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="dcf87-105">Po zobrazení výzvy k přihlášení budete muset použít globální nebo fakturační přihlašovací údaje role správce fakturace.</span><span class="sxs-lookup"><span data-stu-id="dcf87-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="dcf87-106">Pokud nemáte TLS 1,2, může se při pokusu o získání nebo aktualizace zásady zobrazit následující chybová zpráva:</span><span class="sxs-lookup"><span data-stu-id="dcf87-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="dcf87-107">*ErrorMessage – nadřízené připojení bylo uzavřeno: došlo k neočekávané chybě při odeslání*.</span><span class="sxs-lookup"><span data-stu-id="dcf87-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



