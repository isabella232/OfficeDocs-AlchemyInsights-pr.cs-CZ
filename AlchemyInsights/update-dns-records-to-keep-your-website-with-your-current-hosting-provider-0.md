---
title: Aktualizace záznamů DNS tak, aby web zůstal u současného poskytovatele hostingu
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815778"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="9c5df-102">Aktualizace záznamů DNS tak, aby web zůstal u současného poskytovatele hostingu</span><span class="sxs-lookup"><span data-stu-id="9c5df-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="9c5df-103">V centru pro správu Microsoft 365 přejděte na stránku **Nastavení**  >  [domény](https://admin.microsoft.com/Adminportal#/Domains) a v seznamu domén vyberte doménu, kterou používáte pro svůj web.</span><span class="sxs-lookup"><span data-stu-id="9c5df-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="9c5df-104">Vyberte **+ Nový vlastní záznam** a zadejte tyto údaje:</span><span class="sxs-lookup"><span data-stu-id="9c5df-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="9c5df-105">Pro **Typ DNS** zadejte: **A (adresa)**</span><span class="sxs-lookup"><span data-stu-id="9c5df-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="9c5df-106">Jako **Název hostitele nebo alias** zadejte tento symbol: **@**</span><span class="sxs-lookup"><span data-stu-id="9c5df-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="9c5df-107">Do pole **IP adresa** zadejte statickou IP adresu, na které je váš web právě hostovaný (třeba 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="9c5df-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="9c5df-p101">Je nutné, aby to byla  *statická*  IP adresa webu, ne  *dynamická*  IP adresa. Na serveru, kde je web hostovaný, se ujistěte, že pro svůj veřejný web můžete získat statickou IP adresu.</span><span class="sxs-lookup"><span data-stu-id="9c5df-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="9c5df-110">Vyberte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="9c5df-110">Select **Save**.</span></span>

<span data-ttu-id="9c5df-111">Kromě toho můžete vytvořit záznam CNAME, který zákazníkům pomůže váš web najít.</span><span class="sxs-lookup"><span data-stu-id="9c5df-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="9c5df-112">Vyberte **+ Nový vlastní záznam** a zadejte tyto údaje:</span><span class="sxs-lookup"><span data-stu-id="9c5df-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="9c5df-113">Pro **Typ DNS** zadejte: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="9c5df-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="9c5df-114">Do **Název hostitele nebo alias** zadejte: **www**</span><span class="sxs-lookup"><span data-stu-id="9c5df-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="9c5df-115">Do pole **Ukazatel na adresu** zadejte plně kvalifikovaný název domény pro svůj web (třeba contoso.com).</span><span class="sxs-lookup"><span data-stu-id="9c5df-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="9c5df-116">Vyberte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="9c5df-116">Select **Save**.</span></span>
