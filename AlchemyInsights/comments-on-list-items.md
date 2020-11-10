---
title: Komentáře k položkám seznamu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982432"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="ef949-102">Komentáře k položkám seznamu</span><span class="sxs-lookup"><span data-stu-id="ef949-102">Comments on List items</span></span>

<span data-ttu-id="ef949-103">Uživatelé budou brzy moct přidávat a odstraňovat komentáře k položkám seznamu.</span><span class="sxs-lookup"><span data-stu-id="ef949-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="ef949-104">Uživatelé mohou zobrazit všechny komentáře k položce seznamu a filtrovat je mezi zobrazeními, která zobrazují komentáře nebo aktivity související s položkou.</span><span class="sxs-lookup"><span data-stu-id="ef949-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="ef949-105">**Načasování** :</span><span class="sxs-lookup"><span data-stu-id="ef949-105">**Timing** :</span></span>

<span data-ttu-id="ef949-106">**Cílová verze** : postupné Shrnutí v polovině dne a očekávané dokončení v polovině dne</span><span class="sxs-lookup"><span data-stu-id="ef949-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="ef949-107">**Standardní verze** : postupné Shrnutí v polovině dne a očekávané dokončení do brzkého dne</span><span class="sxs-lookup"><span data-stu-id="ef949-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="ef949-108">**Zavedení** : cílová verze pro celou organizaci</span><span class="sxs-lookup"><span data-stu-id="ef949-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="ef949-109">Abyste mohli přidávat a odstraňovat komentáře, musí si uživatelé všimnout následujících informací:</span><span class="sxs-lookup"><span data-stu-id="ef949-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="ef949-110">Komentáře sledují nastavení oprávnění, které jsou součástí SharePointu.</span><span class="sxs-lookup"><span data-stu-id="ef949-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="ef949-111">Klasické seznamy, které ještě nejsou vytvořené pro zobrazení v moderních uživatelských rozhraních, jako jsou seznamy úkolů, tuto funkci komentáře nemají.</span><span class="sxs-lookup"><span data-stu-id="ef949-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="ef949-112">Komentáře k seznamům v aplikaci Teams nejsou k dispozici v této verzi.</span><span class="sxs-lookup"><span data-stu-id="ef949-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="ef949-113">Komentáře nejsou indexovány pomocí vyhledávání.</span><span class="sxs-lookup"><span data-stu-id="ef949-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="ef949-114">Správci můžou tuto funkci na úrovni organizace zakázat změnou parametru **CommentsOnListItemsDisabled** v rutině **set-SPOTenant** PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="ef949-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="ef949-115">V tuto chvíli není možné zakázat komentáře na úrovni webu nebo seznamu.</span><span class="sxs-lookup"><span data-stu-id="ef949-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="ef949-116">Doufáme, že máte tyto kontroly v pozdější aktualizaci, což je pravděpodobné v prvním čtvrtletí 2021.</span><span class="sxs-lookup"><span data-stu-id="ef949-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
