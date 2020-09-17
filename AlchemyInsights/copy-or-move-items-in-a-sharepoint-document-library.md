---
title: Kopírování nebo přesouvání položek v knihovně dokumentů SharePointu
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: d7aa865a6b3db0871a57313dd7d6f5b0213ca0e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807112"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="e80d9-102">Kopírování nebo přesouvání položek v knihovně dokumentů SharePointu</span><span class="sxs-lookup"><span data-stu-id="e80d9-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="e80d9-103">Soubory, složky a odkazy můžete kopírovat a přesouvat do různých umístění v knihovně dokumentů.</span><span class="sxs-lookup"><span data-stu-id="e80d9-103">You can copy and move files, folders, and links to different locations within a document library.</span></span> <span data-ttu-id="e80d9-104">Můžete také kopírovat položky mezi weby.</span><span class="sxs-lookup"><span data-stu-id="e80d9-104">You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="e80d9-105">V prohlížeči přejděte na soubory, složky nebo odkazy, které chcete přesunout, a potom klikněte na **Kopírovat do** nebo **přesunout do**.</span><span class="sxs-lookup"><span data-stu-id="e80d9-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e80d9-106">**Kopírování** a **přesouvání** není dostupné, pokud používáte klasické prostředí SharePointu Online.</span><span class="sxs-lookup"><span data-stu-id="e80d9-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="e80d9-107">V části **Zvolte cíl**vyberte umístění, do kterého chcete položky zkopírovat nebo přesunout, nebo klikněte na **Procházet weby** a zobrazte úplný seznam webů.</span><span class="sxs-lookup"><span data-stu-id="e80d9-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e80d9-108">Pokud nevidíte jiné weby, které jsou uvedené při kopírování položek, kopírování mezi weby není nakonfigurováno.</span><span class="sxs-lookup"><span data-stu-id="e80d9-108">If you don't see other sites listed when you copy items, copying across sites hasn't been configured.</span></span> <span data-ttu-id="e80d9-109">Pokud ho chcete povolit, přejděte na stránku nastavení centra pro správu SharePointu a klikněte na **OK**.</span><span class="sxs-lookup"><span data-stu-id="e80d9-109">To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="e80d9-110">Pokud chcete vytvořit novou složku, vyberte umístění v hierarchii složek, klikněte na **Nová složka**, zadejte název složky a klikněte na značku zaškrtnutí a uložte název.</span><span class="sxs-lookup"><span data-stu-id="e80d9-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="e80d9-111">Klikněte na **Kopírovat sem** nebo **přesunout sem**.</span><span class="sxs-lookup"><span data-stu-id="e80d9-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e80d9-112">Můžete kopírovat až 500 MB souborů a složek najednou.</span><span class="sxs-lookup"><span data-stu-id="e80d9-112">You can copy up to 500 MB of files and folders at one time.</span></span> <span data-ttu-id="e80d9-113">Při kopírování dokumentů s historií verzí se > zkopíruje jenom nejnovější verze.</span><span class="sxs-lookup"><span data-stu-id="e80d9-113">>  When you copy documents that have version history, only the latest version is copied.</span></span> <span data-ttu-id="e80d9-114">Při přesouvání dokumentů se také přesune historie.</span><span class="sxs-lookup"><span data-stu-id="e80d9-114">When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="e80d9-115">Když se soubor přepřesouvá, bude se pořád zobrazovat ve zdrojovém adresáři, dokud se nepřesune do cílového umístění a pak se odstraní.</span><span class="sxs-lookup"><span data-stu-id="e80d9-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="e80d9-116">Soubor zůstane v koši zdrojových webů po dokončení přesouvání a bude podléhat obvyklému plánu recyklace, pokud ho uživatel neobnoví z koše.</span><span class="sxs-lookup"><span data-stu-id="e80d9-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="e80d9-117">Další informace najdete tady:</span><span class="sxs-lookup"><span data-stu-id="e80d9-117">For more information, see:</span></span>

 - <span data-ttu-id="e80d9-118">[Přesouvání nebo kopírování souborů v SharePointu](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (článek podpory Office)</span><span class="sxs-lookup"><span data-stu-id="e80d9-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="e80d9-119">[Přesouvání souborů z libovolné složky](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (článek na blog Microsoft Tech Community)</span><span class="sxs-lookup"><span data-stu-id="e80d9-119">[Move files from any folder](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  