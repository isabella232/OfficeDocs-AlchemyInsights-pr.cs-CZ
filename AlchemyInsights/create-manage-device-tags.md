---
title: Vytváření a správa značek nebo skupin zařízení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731341"
---
# <a name="create-and-manage-device-tags-or-groups"></a>Vytváření a správa značek nebo skupin zařízení

Přidáním značek na zařízeních vytvoříte logickou skupinu. Značky zařízení podporují správné mapování sítě, což umožňuje připojit různé značky k zachycení kontextu a povolit vytváření dynamických seznamu jako součást incidentu. Značky můžete použít jako filtr v zobrazení seznamu Zařízení nebo pro seskupit zařízení. Další informace o seskupování zařízení najdete v tématu [Vytvoření a správa značek zařízení](/microsoft-365/security/defender-endpoint/machine-tags).

Značky na zařízeních můžete přidat pomocí:

- Používání portálu

- Nastavení hodnoty klíče registru
 
**Poznámka:** Mezi přidáním značky na zařízení a jeho dostupností v seznamu zařízení a na stránce zařízení může být latence.

Pokud chcete přidat značky zařízení pomocí rozhraní API, podívejte se na téma [Přidání nebo odebrání značek zařízení API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).

## <a name="add-and-manage-device-tags-using-the-portal"></a>Přidání a správa značek zařízení pomocí portálu

1. Vyberte zařízení, na které chcete spravovat značky. Zařízení můžete vybrat nebo vyhledat v libovolném z následujících zobrazení:

    - **Řídicí panel operací zabezpečení** V části Top devices with active alerts (Nejlepší zařízení s aktivními výstrahami) vyberte název zařízení.
    - **Fronta upozornění** : V frontě upozornění vyberte název zařízení vedle ikony zařízení.
    - **Seznam zařízení** – v seznamu zařízení vyberte název zařízení.
    - **Vyhledávací pole** : V rozevírací nabídce vyberte Zařízení a zadejte název zařízení.

    Můžete se taky dostat na stránku s upozorněním prostřednictvím zobrazení souborů a IP adres.

1. Na **řádku akcí** Odpovědi vyberte Spravovat značky.

1. Pokud chcete najít nebo vytvořit značky, zadejte ho.

Značky se přidávají do zobrazení zařízení a projeví se v zobrazení seznamu Zařízení. Pak můžete pomocí filtru Značky zobrazit příslušný seznam zařízení.

Další informace najdete v tématu [Vytvoření a správa značek zařízení](/microsoft-365/security/defender-endpoint/machine-tags).