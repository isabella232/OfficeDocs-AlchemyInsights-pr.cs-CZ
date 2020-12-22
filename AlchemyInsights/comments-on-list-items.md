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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724147"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="905bb-102">Komentáře k položkám seznamu</span><span class="sxs-lookup"><span data-stu-id="905bb-102">Comments on List items</span></span>

<span data-ttu-id="905bb-103">Uživatelé mohou zobrazit všechny komentáře k položce seznamu a filtrovat je mezi zobrazeními, která zobrazují komentáře nebo aktivity související s položkou.</span><span class="sxs-lookup"><span data-stu-id="905bb-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="905bb-104">Abyste mohli přidávat a odstraňovat komentáře, musí si uživatelé všimnout následujících informací:</span><span class="sxs-lookup"><span data-stu-id="905bb-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="905bb-105">Komentáře sledují nastavení oprávnění, které jsou součástí SharePointu.</span><span class="sxs-lookup"><span data-stu-id="905bb-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="905bb-106">Klasické seznamy, které ještě nejsou vytvořené pro zobrazení v moderních uživatelských rozhraních, jako jsou seznamy úkolů, tuto funkci komentáře nemají.</span><span class="sxs-lookup"><span data-stu-id="905bb-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="905bb-107">Komentáře k seznamům v aplikaci Teams nejsou k dispozici v této verzi.</span><span class="sxs-lookup"><span data-stu-id="905bb-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="905bb-108">Komentáře nejsou indexovány pomocí vyhledávání.</span><span class="sxs-lookup"><span data-stu-id="905bb-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="905bb-109">Správci můžou tuto funkci na úrovni organizace zakázat změnou parametru **CommentsOnListItemsDisabled** v rutině **set-SPOTenant** PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="905bb-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="905bb-110">V tuto chvíli není možné zakázat komentáře na úrovni webu nebo seznamu.</span><span class="sxs-lookup"><span data-stu-id="905bb-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="905bb-111">Doufáme, že máte tyto kontroly v pozdější aktualizaci, což je pravděpodobné v prvním čtvrtletí 2021.</span><span class="sxs-lookup"><span data-stu-id="905bb-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
