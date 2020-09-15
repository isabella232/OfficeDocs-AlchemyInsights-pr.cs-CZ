---
title: Dynamics 365 – chybný řídicí panel v rozhraní Dynamics 365 Unified
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711268"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Chybný řídicí panel zobrazený v aplikaci Dynamics 365 Unified Interface

Existuje několik důvodů, proč se může zobrazit jiný řídicí panel, než očekáváte:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Uživatel nastavil výchozí uživatelský řídicí panel 

Výchozí uživatelský řídicí panel se obvykle dá nastavit, pokud se na panelu příkazů řídicí panel nezobrazí tlačítko **nastavit jako výchozí** . Výchozí řídicí panel uživatele přepíše všechny ostatní výchozí řídicí panely, a to i v případě, že výchozí řídicí panel uživatele není aktuální aplikací.

Pomocí následujícího zástupného řešení zrušte výchozí řídicí panel.

1. Vytvořte nový osobní řídicí panel.

2. Nastavte si nový řídicí panel jako výchozí.

3. Odstraňte tento řídicí panel.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>V prvku Sitemap je nastaven řídicí panel

Možná jste nastavili výchozí řídicí panel organizace výběrem řídicího panelu a zvolením možnosti nastavit jako výchozí v části přizpůsobit systém. Ale řídicí panel definovaný v Návrháři mapy webu bude mít při přístupu k tomuto řídicímu panelu přednost.

Pokud chcete, aby uživatelé viděli řídicí panel, který jste nastavili jako výchozí, můžete:

* Nastavení tohoto řídicího panelu v článku Mapa stránek

* Odebrání přístupu k řídicímu panelu mapy webu pro tyto uživatele
