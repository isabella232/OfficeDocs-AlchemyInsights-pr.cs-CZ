---
title: Vytváření a sdílení kalendářů veřejných složek v Exchangi Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: d8b28d373db21da42b90aeef75139affd802a5d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47803538"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a><span data-ttu-id="54491-102">Vytváření a sdílení kalendářů veřejných složek v Exchangi Online</span><span class="sxs-lookup"><span data-stu-id="54491-102">Create and share public folder calendars in Exchange Online</span></span>

<span data-ttu-id="54491-103">Kalendář ve veřejné složce můžete vytvořit jenom z desktopového klienta Outlooku.</span><span class="sxs-lookup"><span data-stu-id="54491-103">You can create a calendar in the Public folder only from the Outlook desktop client.</span></span> <span data-ttu-id="54491-104">K nastavení kalendářů veřejné složky použijte tento postup:</span><span class="sxs-lookup"><span data-stu-id="54491-104">Use these steps to set up public folder calendars:</span></span>

1. <span data-ttu-id="54491-105">Zajistěte, aby byly veřejné složky nasazené v Exchangi Online.</span><span class="sxs-lookup"><span data-stu-id="54491-105">Ensure public folders are deployed in Exchange Online.</span></span> <span data-ttu-id="54491-106">Další informace najdete v tématu [Vytvoření poštovní schránky veřejné složky](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span><span class="sxs-lookup"><span data-stu-id="54491-106">For more info, see [Create a public folder mailbox](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span></span> 

2. <span data-ttu-id="54491-107">Zkontrolujte, jestli máte přiřazená potřebná přístupová oprávnění k vytvoření veřejné složky.</span><span class="sxs-lookup"><span data-stu-id="54491-107">Ensure you're assigned necessary access permissions to create the public folder.</span></span> <span data-ttu-id="54491-108">Další informace najdete v článku [oprávnění k veřejným složkám pro Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="54491-108">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span> 
  
3. <span data-ttu-id="54491-109">Přihlaste se do desktopového klienta Outlooku a zkontrolujte, jestli máte přístup k nasazení veřejné složky.</span><span class="sxs-lookup"><span data-stu-id="54491-109">Log in to the Outlook desktop client and ensure you can access your public folder deployment.</span></span>

    <span data-ttu-id="54491-110">Pokud máte potíže s přístupem k veřejným složkám pomocí desktopového klienta Outlooku, přečtěte si článek [Exchange Online uživatelé se nemohou připojit k veřejným složkám pomocí Outlooku nebo OWA](https://aka.ms/pfcte).</span><span class="sxs-lookup"><span data-stu-id="54491-110">If you're having trouble accessing public folders by using the Outlook desktop client, see [Exchange Online users can't connect to public folders by using Outlook or OWA](https://aka.ms/pfcte).</span></span>

4. <span data-ttu-id="54491-111">Vytvořte nový typ kalendáře veřejné složky.</span><span class="sxs-lookup"><span data-stu-id="54491-111">Create a new public folder calendar type.</span></span>

<span data-ttu-id="54491-112">Veřejná složka je ve výchozím nastavení sdílená s ostatními uživateli.</span><span class="sxs-lookup"><span data-stu-id="54491-112">The public folder is shared to all other users by default.</span></span> <span data-ttu-id="54491-113">Vlastník veřejné složky může změnit oprávnění pro desktopového klienta Outlooku.</span><span class="sxs-lookup"><span data-stu-id="54491-113">Owner of the public folder can change the permissions from Outlook desktop client.</span></span> <span data-ttu-id="54491-114">Další informace najdete v článku [oprávnění k veřejným složkám pro Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="54491-114">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span>

<span data-ttu-id="54491-115">**Poznámka:** Kalendáře veřejné složky jsou navržené tak, aby se používaly v organizaci a nedají se publikovat na internetu.</span><span class="sxs-lookup"><span data-stu-id="54491-115">**Note** Public folder calendars are designed to be used within the organization and can't be published on the Internet.</span></span> <span data-ttu-id="54491-116">Pokud chcete publikovat kalendář na internetu, použijte sdílenou poštovní schránku.</span><span class="sxs-lookup"><span data-stu-id="54491-116">Use a shared mailbox if your intention is to publish a calendar on the  Internet.</span></span>