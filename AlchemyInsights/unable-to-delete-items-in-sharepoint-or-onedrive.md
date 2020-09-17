---
title: Nelze odstranit položky na SharePointu nebo OneDrivu.
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806104"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="e2495-102">Nelze odstranit položky</span><span class="sxs-lookup"><span data-stu-id="e2495-102">Unable to delete items</span></span>

<span data-ttu-id="e2495-103">Zásady uchovávání informací mohou způsobit, že je nutné zakázat nebo vyloučit odpovídající blokování, které je příčinou tohoto problému.</span><span class="sxs-lookup"><span data-stu-id="e2495-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="e2495-104">Po odebrání zásad uchovávání informací nebo držení může trvat až 24 hodin, než se změna projeví.</span><span class="sxs-lookup"><span data-stu-id="e2495-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="e2495-105">Ujistěte se, že u položky neexistuje nastavení [zásad uchovávání informací](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) .</span><span class="sxs-lookup"><span data-stu-id="e2495-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="e2495-106">Web mohl mít překročen limit úložiště, zvýšit [kvótu webu](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) a odstranit položku.</span><span class="sxs-lookup"><span data-stu-id="e2495-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="e2495-107">Ujistěte se, že položka není [rezervována](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) pro jiného uživatele.</span><span class="sxs-lookup"><span data-stu-id="e2495-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="e2495-108">Správci můžou použít [vzory a postupy SharePointu](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) , které obsahují knihovnu příkazů PowerShellu, které umožňují provádět složité akce správy, jako je například vynutit odstranění stubborn položek.</span><span class="sxs-lookup"><span data-stu-id="e2495-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="e2495-109">Odebrání souboru PNP</span><span class="sxs-lookup"><span data-stu-id="e2495-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="e2495-110">Odebrání složky PNP</span><span class="sxs-lookup"><span data-stu-id="e2495-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="e2495-111">Odebrání položky seznamu PNP</span><span class="sxs-lookup"><span data-stu-id="e2495-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="e2495-112">Odebrat seznam PNP</span><span class="sxs-lookup"><span data-stu-id="e2495-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="e2495-113">Odebrání pole PNP (sloupec)</span><span class="sxs-lookup"><span data-stu-id="e2495-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)