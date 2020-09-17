---
title: Obnovení odstraněného souboru nebo složky
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: fc560686ec5c6a3d42a97687fda80ae5001b5c60
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797541"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="5d52c-102">Obnovení odstraněného souboru nebo složky</span><span class="sxs-lookup"><span data-stu-id="5d52c-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="5d52c-103">SharePoint Online zachovává zálohy veškerého obsahu ještě 14 dnů po jeho vlastním odstranění.</span><span class="sxs-lookup"><span data-stu-id="5d52c-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="5d52c-104">Pokud nelze obsah obnovit pomocí koše nebo obnovení souborů, může správce kontaktovat podporu Microsoftu, požádat o obnovení kdykoli v okně 14 dní.</span><span class="sxs-lookup"><span data-stu-id="5d52c-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="5d52c-105">Obnovení ze záloh se dá realizovat jenom pro kolekce webů nebo podřízené weby, ale ne pro konkrétní soubory, seznamy nebo knihovny.</span><span class="sxs-lookup"><span data-stu-id="5d52c-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="5d52c-106">Když odstraníte položku nebo web ze SharePointu, není okamžitě odebrán.</span><span class="sxs-lookup"><span data-stu-id="5d52c-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="5d52c-107">Odstraněné položky se na určitou dobu přesunou do koše.</span><span class="sxs-lookup"><span data-stu-id="5d52c-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="5d52c-108">Během této doby můžete odstraněné položky obnovit v původním umístění.</span><span class="sxs-lookup"><span data-stu-id="5d52c-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="5d52c-109">Pokud chcete získat další informace, podívejte se na níže uvedené odkazy.</span><span class="sxs-lookup"><span data-stu-id="5d52c-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="5d52c-110">[Obnovení položek v odpadkovém koši webu SharePointu](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b)</span><span class="sxs-lookup"><span data-stu-id="5d52c-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="5d52c-111">Obnovení odstraněných souborů nebo složek na OneDrivu</span><span class="sxs-lookup"><span data-stu-id="5d52c-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="5d52c-112">Obnovení odstraněné kolekce webů (včetně skupiny, komunikace a dalších webů)</span><span class="sxs-lookup"><span data-stu-id="5d52c-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="5d52c-113">Obnovení odstraněného webu OneDrivu</span><span class="sxs-lookup"><span data-stu-id="5d52c-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="5d52c-114">U akcí v hromadném koši můžou správci zvážit použití [pnp v SharePointu Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="5d52c-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="5d52c-115">**Funkce pro obnovení souborů**</span><span class="sxs-lookup"><span data-stu-id="5d52c-115">**Files Restore feature**</span></span>

<span data-ttu-id="5d52c-116">Pokud se hodně vašich souborů na OneDrivu nebo SharePointu odstraní, přepíší, jsou poškozené nebo jsou nakaženy malwarem, můžete obnovit původní knihovnu OneDrivu nebo SharePointu v předchozí verzi pomocí funkce obnovení souborů.</span><span class="sxs-lookup"><span data-stu-id="5d52c-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="5d52c-117">Obnovení knihovny OneDrivu</span><span class="sxs-lookup"><span data-stu-id="5d52c-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="5d52c-118">Obnovení knihovny dokumentů</span><span class="sxs-lookup"><span data-stu-id="5d52c-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

