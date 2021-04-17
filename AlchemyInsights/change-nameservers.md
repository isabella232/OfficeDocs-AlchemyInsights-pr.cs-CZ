---
title: Změna názvových serverů
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818605"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="cf73c-102">Aktualizace názvových serverů domény, aby odkazovaly na Microsoft</span><span class="sxs-lookup"><span data-stu-id="cf73c-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="cf73c-103">Poznámka: Rozšíření změn názvových serverů může v některých případech trvat až 48 hodin.</span><span class="sxs-lookup"><span data-stu-id="cf73c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="cf73c-p101">Když si nastavujete doménu v Microsoftu 365, je nutné aktualizovat názvové servery u vašeho registrátora. Vytvořte nebo upravte záznamy názvových serverů u svého doménového registrátora.</span><span class="sxs-lookup"><span data-stu-id="cf73c-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="cf73c-106">Přejděte web svého doménového registrátora a najděte část, kde můžete upravovat názvové servery.</span><span class="sxs-lookup"><span data-stu-id="cf73c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="cf73c-107">Vytvořte nebo upravte dva záznamy názvových serverů, aby se shodovaly s těmito hodnotami:</span><span class="sxs-lookup"><span data-stu-id="cf73c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="cf73c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="cf73c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="cf73c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="cf73c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="cf73c-110">Uložte změny.</span><span class="sxs-lookup"><span data-stu-id="cf73c-110">Save changes.</span></span>

<span data-ttu-id="cf73c-111">Podrobné pokyny najdete i v tomto článku, který se věnuje [změně názvových serverů u libovolného doménového registrátora](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span><span class="sxs-lookup"><span data-stu-id="cf73c-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  