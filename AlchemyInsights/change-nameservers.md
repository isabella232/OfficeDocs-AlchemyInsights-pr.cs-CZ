---
title: Změna názvových serverů
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f295e0d7872a13cf47e386343b159e51bc0504de
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508081"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="e20a5-102">Aktualizace názvových serverů domény, aby odkazovaly na Microsoft</span><span class="sxs-lookup"><span data-stu-id="e20a5-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="e20a5-103">Poznámka: Rozšíření změn názvových serverů může v některých případech trvat až 48 hodin.</span><span class="sxs-lookup"><span data-stu-id="e20a5-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="e20a5-p101">Když si nastavujete doménu v Microsoftu 365, je nutné aktualizovat názvové servery u vašeho registrátora. Vytvořte nebo upravte záznamy názvových serverů u svého doménového registrátora.</span><span class="sxs-lookup"><span data-stu-id="e20a5-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="e20a5-106">Přejděte web svého doménového registrátora a najděte část, kde můžete upravovat názvové servery.</span><span class="sxs-lookup"><span data-stu-id="e20a5-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="e20a5-107">Vytvořte nebo upravte dva záznamy názvových serverů, aby se shodovaly s těmito hodnotami:</span><span class="sxs-lookup"><span data-stu-id="e20a5-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="e20a5-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e20a5-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="e20a5-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e20a5-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="e20a5-110">Uložte změny.</span><span class="sxs-lookup"><span data-stu-id="e20a5-110">Save changes.</span></span>

<span data-ttu-id="e20a5-111">Podrobné pokyny najdete i v tomto článku, který se věnuje [změně názvových serverů u libovolného doménového registrátora](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span><span class="sxs-lookup"><span data-stu-id="e20a5-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  