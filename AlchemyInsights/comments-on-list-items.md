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
# <a name="comments-on-list-items"></a>Komentáře k položkám seznamu

Uživatelé budou brzy moct přidávat a odstraňovat komentáře k položkám seznamu. Uživatelé mohou zobrazit všechny komentáře k položce seznamu a filtrovat je mezi zobrazeními, která zobrazují komentáře nebo aktivity související s položkou.

**Načasování** :

**Cílová verze** : postupné Shrnutí v polovině dne a očekávané dokončení v polovině dne

**Standardní verze** : postupné Shrnutí v polovině dne a očekávané dokončení do brzkého dne

**Zavedení** : cílová verze pro celou organizaci

Abyste mohli přidávat a odstraňovat komentáře, musí si uživatelé všimnout následujících informací:

- Komentáře sledují nastavení oprávnění, které jsou součástí SharePointu.
- Klasické seznamy, které ještě nejsou vytvořené pro zobrazení v moderních uživatelských rozhraních, jako jsou seznamy úkolů, tuto funkci komentáře nemají.
- Komentáře k seznamům v aplikaci Teams nejsou k dispozici v této verzi.
- Komentáře nejsou indexovány pomocí vyhledávání.

Správci můžou tuto funkci na úrovni organizace zakázat změnou parametru **CommentsOnListItemsDisabled** v rutině **set-SPOTenant** PowerShellu.

V tuto chvíli není možné zakázat komentáře na úrovni webu nebo seznamu. Doufáme, že máte tyto kontroly v pozdější aktualizaci, což je pravděpodobné v prvním čtvrtletí 2021.
