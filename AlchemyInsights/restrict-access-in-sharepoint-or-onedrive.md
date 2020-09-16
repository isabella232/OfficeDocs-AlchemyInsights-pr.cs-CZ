---
title: Omezení přístupu v SharePointu nebo OneDrivu
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720675"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="56d6e-102">Omezení přístupu v SharePointu nebo OneDrivu</span><span class="sxs-lookup"><span data-stu-id="56d6e-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="56d6e-103">V SharePointu a OneDrivu omezíte přístup k položkám, jako jsou soubory, složky a seznamy, udělením přístupu jenom skupinám nebo jednotlivcům, kterým chcete mít přístup.</span><span class="sxs-lookup"><span data-stu-id="56d6e-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="56d6e-104">Ve výchozím nastavení jsou oprávnění v SharePointu zděděná od vyšší úrovně v hierarchii.</span><span class="sxs-lookup"><span data-stu-id="56d6e-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="56d6e-105">Aby soubor zdědil oprávnění ze složky, což dědí oprávnění z knihovny, což dědí oprávnění od webu.</span><span class="sxs-lookup"><span data-stu-id="56d6e-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="56d6e-106">Můžete sdílet na vyšší úrovni (například sdílením celého webu) a přerušit dědičnost, pokud nechcete sdílet všechny položky na webu.</span><span class="sxs-lookup"><span data-stu-id="56d6e-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="56d6e-107">Tento postup ale nedoporučujeme, protože v budoucnu je udržování oprávnění složitější a matoucí.</span><span class="sxs-lookup"><span data-stu-id="56d6e-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="56d6e-108">Co můžete dělat místo:</span><span class="sxs-lookup"><span data-stu-id="56d6e-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="56d6e-109">Pokud chcete například sdílet veškerý obsah složky s výjimkou jednoho souboru, přesuňte tento soubor do nového umístění, které není sdílené.</span><span class="sxs-lookup"><span data-stu-id="56d6e-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="56d6e-110">Pokud složka obsahuje dvě podsložky a chcete sdílet jednu podsložku se skupinami a a B a povolit skupině přístup jenom k druhé podsložce, nasdílejte nadřazenou složku se skupinou A a přidejte skupinu B do první podsložky.</span><span class="sxs-lookup"><span data-stu-id="56d6e-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="56d6e-111">Ukončení sdílení souboru nebo složky </span><span class="sxs-lookup"><span data-stu-id="56d6e-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

