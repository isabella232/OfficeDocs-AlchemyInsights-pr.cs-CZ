---
title: SharePoint velké seznamy
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
ms.openlocfilehash: c67632e323f2068faba06779b94ba4fd8e9f319e18cefb7977bd3038ca770210
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53941561"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Práce s velkými seznamy a knihovnami v SharePoint

SharePoint a knihovny můžou obsahovat až 30 milionů položek, ale pokud mají víc než 5 000 položek, může se při pokusu o práci s nimi zobrazit chyba Mezní hodnota zobrazení seznamu. Tato mezní hodnota slouží k udržování výkonu služby. Nejde změnit. Abyste se vyhnuli překročení této mezní hodnoty:

**Použití moderních**

Zobrazení zobrazující mnoho položek funguje v moderním prostředí nejlépe. [V moderním prostředí se můžete vyhnout](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) chybám, které se můžou v klasickém prostředí zobrazit.

**Přidání indexů**

Při filtrování nebo řazení podle sloupce, který nemá index, se může zobrazit chybová zpráva. [Přidejte index ručně](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) ze **seznamu Nastavení** v nabídce nastavení a pak **Indexované sloupce**.

**Úprava zobrazení seznamu**

Pokud při práci s velkým seznamem dojde k chybě, [upravte zobrazení seznamu](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

Následující čtyři změny odeberou chyby mezní hodnoty zobrazení seznamu. Pokud chcete odebrat všechny chyby, proveďte všechny čtyři změny. Pokud stále dochází k chybám, podívejte se na [Spravovat velké seznamy a knihovny](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).

1. V **seznamu** Nejdřív **seřadit podle sloupce a** Potom seřadit podle sloupce vyberte **Žádné.**
2. V **obou** **sloupci First group by the column** (Žádné) a Then group by the column **(Potom seskupit podle sloupce) vyberte None (Žádné)** z možnosti First group by the column (První skupina podle sloupce) a Then group by the
3. U **všech** sloupců v části Souhrny **vyberte** Žádný.
4. V části Sloupce zrušte zaškrtnutí všech sloupců, ale jenom **jednoho** sloupce.

