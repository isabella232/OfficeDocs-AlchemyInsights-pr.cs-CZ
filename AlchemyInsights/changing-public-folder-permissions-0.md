---
title: Změna oprávnění pro veřejnou složku
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: a2a902e8fdfd8628772364c173979c633d25a169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714240"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="49324-102">Změna oprávnění pro veřejnou složku</span><span class="sxs-lookup"><span data-stu-id="49324-102">Changing public folder permissions</span></span>

<span data-ttu-id="49324-103">Oprávnění pro veřejnou složku můžou měnit uživatelé a správci Outlooku.</span><span class="sxs-lookup"><span data-stu-id="49324-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="49324-104">Správci můžou taky řídit oprávnění v centru pro správu Exchange (EAC):</span><span class="sxs-lookup"><span data-stu-id="49324-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="49324-105">V centru pro správu Microsoft 365 přejděte na Exchange **Centers** \> **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="49324-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="49324-106">Vyberte **veřejné složky**.</span><span class="sxs-lookup"><span data-stu-id="49324-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="49324-107">Odtud můžete změnit oprávnění pro jednotlivé veřejné složky tím, že jim přiřadíte oprávnění.</span><span class="sxs-lookup"><span data-stu-id="49324-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="49324-108">Aby koncový uživatel změnil oprávnění pro veřejnou složku, musí mít pro tuto složku oprávnění vlastníka.</span><span class="sxs-lookup"><span data-stu-id="49324-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="49324-109">Postupujte podle pokynů uvedených v části [Diagnostika a oprava problémů s oprávněními k veřejným složkám](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) s problémy s oprávněními k veřejným složkám.</span><span class="sxs-lookup"><span data-stu-id="49324-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="49324-110">**Poznámka**: při pokusu o změnu oprávnění ve veřejných složkách se může vyskytnout několik známých problémů.</span><span class="sxs-lookup"><span data-stu-id="49324-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="49324-111">Další informace najdete v následujících článcích.</span><span class="sxs-lookup"><span data-stu-id="49324-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="49324-112">V EAC se nedají použít oprávnění u podsložek veřejné složky.</span><span class="sxs-lookup"><span data-stu-id="49324-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="49324-113">Chyba "poštovní schránka se nenašla v místní doménové struktuře" při přístupu do veřejných složek</span><span class="sxs-lookup"><span data-stu-id="49324-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
