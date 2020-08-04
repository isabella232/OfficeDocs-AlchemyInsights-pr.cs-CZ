---
title: Vzdálená správa zařízení Intune pomocí teamvieweru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554840"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Vzdálená správa zařízení Intune pomocí teamvieweru

Zařízení spravovaná službou Intune lze spravovat vzdáleně pomocí [aplikace TeamViewer](https://www.teamviewer.com/).

Chcete-li spravovat Intune pomocí teamvieweru, postupujte takto: 

Začněte získáním přihlašovacích údajů od teamvieweru a nastavte konektor TeamViewer v Intune. To umožňuje správci zadat přihlašovací údaje v uživatelském rozhraní konektoru TeamViewer v části Zařízení, což je jednorázová operace k vytvoření propojení mezi Intune a službou TeamViewer.

**Část 1: Zahájení relace se vzdáleným zařízením**

1. V části **Všechna zařízení**vyberte zařízení, se kterým chcete spustit vzdálenou relaci.
2. Od **... Další**možnost – vyberte **možnost Nová relace vzdálené pomoci**.
3. Vyberte **Ano,** chcete-li potvrdit, že chcete vytvořit vzdálenou relaci.
    Po "Zahájení nové vzdálené relace" požadavek je potvrzena službou TeamViewer, uvidíte možnost **zahájit vzdálenou pomoc** v podrobnostech přehled (nebo Essentials) podokno pro zařízení. Výběrem **možnosti Zobrazit další** rozbalíte podokno a zobrazíte stav vzdálená pomoc.
4. Chcete-li zahájit relaci na straně správce, vyberte **možnost Spustit vzdálenou relaci.**
5. Zvolte stažení binárního souboru TeamViewer (Windows) a vyberte **spustit**.<br/>
    **Poznámka:** Můžete ignorovat libovolnou stránku webového prohlížeče otevřenou na webu TeamViewer.

6. Potvrďte požadavek, aby aplikace TeamViewer v zařízení provádět změny (pouze windows).
7. Aplikace TeamViewer se spustí a obsahuje kód relace pro ověření připojení ke vzdálenému zařízení.

**Část 2: Na zařízení, které je cílené pro vzdálenou relaci**

1. Otevřete portál společnosti Intune.
2. Vyhledejte příznak oznámení: "Správce IT požaduje řízení tohoto zařízení pro relaci vzdálené pomoci" a vyberte oznámení.
3. Zvolte stažení aplikace TeamViewer nebo potvrzením stažení aplikace TeamViewer z obchodu s aplikacemi a vyberte **Spustit**.
    **Poznámka:** Můžete ignorovat libovolnou stránku webového prohlížeče otevřenou na webu TeamViewer.

4. Potvrďte požadavek, aby aplikace TeamViewer v zařízení provádět změny (pouze windows).
5. Aplikace TeamViewer se spustí a obsahuje kód relace pro ověření připojení ke vzdálenému zařízení.
6. Vyskakovací okno se zeptá, zda chcete povolit spuštění relace.

**Poznámka:** Kódy relace generované službou TeamViewer jsou pouze jednorázové použití. Pokud připojení ztratíte, musíte:

1. Zavřete instanci aplikace TeamViewer na vzdáleném zařízení a na pracovní stanici správce.
2. Zavřete portál společnosti na vzdáleném zařízení.
3. Spusťte novou "Novou relaci vzdálené pomoci" z portálu pro správu.
4. Znovu otevřete portál společnosti na vzdáleném zařízení a obdržíte nové oznámení.
5. Stáhněte a otevřete aplikaci TeamViewer na vzdáleném zařízení i na pracovní stanici správce, jako dříve.