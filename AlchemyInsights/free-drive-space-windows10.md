---
title: Volného místa na disku ve Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035668"
---
# <a name="free-up-drive-space-in-windows-10"></a>Volného místa na disku ve Windows 10

Tady jsou dvě možnosti, jak ve Windows volného místa na disku:

- Volná místa na disku ve Windows 10
- Volná místa pro aktualizace Windows 10 s externím úložným zařízením

Pokud máte po použití nástroje Vyčištění disku pořád málo místa na disku, je možné, že složka Temp se rychle zaplní soubory aplikací (.appx), které používá Microsoft Store. Pokud chcete tento problém vyřešit, obnovte Store, vymažte mezipaměť Storu a spusťte Poradce při potížích se službou Windows Update. Než budete pokračovat v těchto krocích, ujistěte se, že je Microsoft Store zavřený.

**Krok 1: Resetování Microsoft Storu**

**Poznámka:** Tím se trvale odstraní data aplikace na zařízení, včetně vašich předvoleb a přihlašovacích údajů.

1. Vyberte **Start**  >  **Settings**  >  **Apps**  >  **Apps & funkce**.

1. V seznamu aplikací vyhledejte a vyberte Microsoft Store.

1. Vyberte **Upřesnit možnosti**.

1. Posuňte se dolů, **vyberte Obnovit a** pak **Potvrdit obnovení továrního nastavení.**

**Krok 2: Vymazání mezipaměti Microsoft Storu**

1. Stisknutím klávesy s logem Windows + R otevřete dialogové okno Spustit.

1. Zadejte wsreset.exe a vyberte **OK**.

1. Otevře se prázdné okno příkazového řádku. Po přibližně 10 sekundách se okno zavře a Store se otevře automaticky.

**Krok 3: Resetování služby Windows Update**

1. Vyberte **Spustit**  >  **aktualizace nastavení** a & poradce při  >  **potížích se**  >  **zabezpečením**.

1. Posuňte se dolů a v seznamu vyberte **Windows Update** a vyberte Spustit poradce **při potížích.**

1. Restartujte počítač a zkontrolujte, jestli k problému stále dochází.

