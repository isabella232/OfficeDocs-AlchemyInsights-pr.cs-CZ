---
title: Rozsáhlé seznamy SharePointu
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
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720126"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="7d199-102">Práce s rozsáhlými seznamy a knihovnami v SharePointu</span><span class="sxs-lookup"><span data-stu-id="7d199-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="7d199-103">Seznamy a knihovny SharePointu můžou obsahovat až 30 000 000 položek, ale pokud mají víc než 5 000 položek, může se při pokusu o práci s nimi zobrazit chybová prahová hodnota zobrazení seznamu.</span><span class="sxs-lookup"><span data-stu-id="7d199-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="7d199-104">Tato mezní hodnota slouží k udržování výkonu služby.</span><span class="sxs-lookup"><span data-stu-id="7d199-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="7d199-105">Nejde změnit.</span><span class="sxs-lookup"><span data-stu-id="7d199-105">It can't be changed.</span></span> <span data-ttu-id="7d199-106">Chcete-li se vyhnout této hranici:</span><span class="sxs-lookup"><span data-stu-id="7d199-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="7d199-107">**Používat moderní**</span><span class="sxs-lookup"><span data-stu-id="7d199-107">**Use modern**</span></span>

<span data-ttu-id="7d199-108">Zobrazení s velkým množstvím položek fungují nejlépe v moderních prostředích.</span><span class="sxs-lookup"><span data-stu-id="7d199-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="7d199-109">[Využijte moderní prostředí](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) pro předcházení chybám, které se můžou objevit v klasickém prostředí.</span><span class="sxs-lookup"><span data-stu-id="7d199-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="7d199-110">**Přidání indexů**</span><span class="sxs-lookup"><span data-stu-id="7d199-110">**Add indexes**</span></span>

<span data-ttu-id="7d199-111">Při filtrování nebo řazení podle sloupce, který nemá index, se může zobrazit chybová zpráva.</span><span class="sxs-lookup"><span data-stu-id="7d199-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="7d199-112">[Přidejte index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) ručně ze **seznamu nastavení** v nabídce nastavení a potom klikněte na **indexované sloupce**.</span><span class="sxs-lookup"><span data-stu-id="7d199-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="7d199-113">**Úprava zobrazení seznamu**</span><span class="sxs-lookup"><span data-stu-id="7d199-113">**Edit the list view**</span></span>

<span data-ttu-id="7d199-114">Pokud při práci s rozsáhlým seznamem dojde k chybě, [upravte zobrazení seznamu](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="7d199-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="7d199-115">V následujících čtyřech změnách dojde k odebrání chyb mezních hodnot zobrazení seznamu.</span><span class="sxs-lookup"><span data-stu-id="7d199-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="7d199-116">Všechny čtyři změny se projeví po odebrání všech chyb.</span><span class="sxs-lookup"><span data-stu-id="7d199-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="7d199-117">Pokud se vám pořád zobrazují chyby, zaškrtněte políčko [Spravovat rozsáhlé seznamy a knihovny](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="7d199-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="7d199-118">Chcete-li v obou případech vybrat možnost **žádné** , **seřaďte oba sloupce** a **potom seřaďte sloupec**.</span><span class="sxs-lookup"><span data-stu-id="7d199-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="7d199-119">Vyberte **žádné** z **první skupiny podle sloupce** a **potom seskupení podle sloupce**.</span><span class="sxs-lookup"><span data-stu-id="7d199-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="7d199-120">V části **souhrny** vyberte **žádné** .</span><span class="sxs-lookup"><span data-stu-id="7d199-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="7d199-121">V části **sloupce** zrušte výběr všech sloupců kromě jednoho.</span><span class="sxs-lookup"><span data-stu-id="7d199-121">Deselect all but one column for display from the **Columns** section.</span></span>

