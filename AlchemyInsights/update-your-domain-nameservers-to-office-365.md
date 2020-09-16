---
title: Aktualizace názvových serverů domény, aby odkazovaly na Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734904"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="a1ed7-102">Aktualizace názvových serverů domény, aby odkazovaly na Microsoft</span><span class="sxs-lookup"><span data-stu-id="a1ed7-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="a1ed7-103">Poznámka: Rozšíření změn názvových serverů může v některých případech trvat až 48 hodin.</span><span class="sxs-lookup"><span data-stu-id="a1ed7-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="a1ed7-104">Chcete-li nastavit doménu u společnosti Microsoft, je třeba aktualizovat názvové servery v registrátorovi.</span><span class="sxs-lookup"><span data-stu-id="a1ed7-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="a1ed7-105">Vytvořte nebo upravte záznamy názvových serverů u svého doménového registrátora.</span><span class="sxs-lookup"><span data-stu-id="a1ed7-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="a1ed7-106">Přejděte web svého doménového registrátora a najděte část, kde můžete upravovat názvové servery.</span><span class="sxs-lookup"><span data-stu-id="a1ed7-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="a1ed7-107">Vytvořte nebo upravte dva záznamy názvových serverů, aby se shodovaly s těmito hodnotami:</span><span class="sxs-lookup"><span data-stu-id="a1ed7-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="a1ed7-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a1ed7-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="a1ed7-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a1ed7-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="a1ed7-110">Uložte změny.</span><span class="sxs-lookup"><span data-stu-id="a1ed7-110">Save changes.</span></span>

<span data-ttu-id="a1ed7-111">Podrobné pokyny najdete také v tomto článku: [Změna názvové servery na nastavení systému Microsoft 365 s libovolným doménovým registrátorem](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="a1ed7-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  