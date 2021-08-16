---
title: Dynamics 365 – nesprávné zobrazení řídicího panelu v jednotném rozhraní Dynamics 365
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
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101475"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>V jednotném rozhraní Dynamics 365 se zobrazuje nesprávný řídicí panel.

Existuje několik důvodů, proč se může zobrazit jiný řídicí panel, než který očekáváte:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Uživatel nastavil výchozí řídicí panel uživatele. 

Obvykle můžete určit, že výchozí řídicí  panel uživatele je nastavený, pokud se tlačítko Nastavit jako výchozí na panelu příkazů řídicího panelu nezminí. Výchozí řídicí panel uživatele přepíše všechny ostatní výchozí řídicí panely, i když výchozí řídicí panel uživatele není v aktuální aplikaci.

Pokud chcete zrušit výchozí řídicí panel, použijte následující alternativní řešení.

1. Vytvořte nový osobní řídicí panel.

2. Nastavte tento nový řídicí panel jako výchozí nastavení uživatele.

3. Odstraňte tento řídicí panel.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Řídicí panel je nastavený v mapě webu.

Výchozí řídicí panel organizace jste možná nastavili tak, že vyberete řídicí panel a v části Přizpůsobit systém zvolíte Nastavit jako výchozí. Řídicí panel definovaný v návrháři mapy webu ale bude mít přednost před tímto řídicím panelem, pokud k tomu má uživatel přístup.

Pokud chcete, aby uživatelé viděli řídicí panel, který jste nastavili jako výchozí nastavení organizace, můžete buď:

* Nastavení řídicího panelu v mapě webu

* Odebrání přístupu k řídicímu panelu definovanému v souboru Sitemap pro tyto uživatele
