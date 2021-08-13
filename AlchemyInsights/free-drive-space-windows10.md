---
title: Uvolnění místa na disku ve Windows 10
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: c7d29ab718be8dbdcde61a7de2f158fb3bbd722d2964d8b13cde9936dd1e5ee1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928074"
---
# <a name="free-up-drive-space-in-windows-10"></a>Uvolnění místa na disku ve Windows 10

Tady jsou dvě možnosti, jak uvolnit místo na disku ve Windows:

- Uvolnění místa na disku ve Windows 10.
- Uvolněte místo pro aktualizace Windows 10 s pomocí externího úložiště.

Pokud máte po použití nástroje Vyčištění disku stále málo místa, je možné, že se vaše složka Temp rychle plní soubory aplikací (.appx), které používá Microsoft Store. Tento problém vyřešíte resetováním Microsoft Store, vymazáním mezipaměti Microsoft Store a spuštěním poradce při potížích služby Windows Update. Zavřete Microsoft Store předtím, než se pustíte do těchto kroků.

**Krok 1: Resetujte Microsoft Store**

**Poznámka** Tímto krokem dojde k trvalému smazání dat aplikace na zařízení, včetně vašich předvoleb a přihlašovacích údajů.

1. Vyberte **Start** > **Nastavení** > **Aplikace** > **Aplikace a funkce**.

1. V seznamu aplikací najděte a vyberte Microsoft Store.

1. Vyberte **Upřesnit možnosti**.

1. Posuňte se dolů a vyberte **Resetovat** a pak **Potvrdit resetování**.

**Krok 2: Vymažte mezipaměť Microsoft Store**

1. Stisknutím klávesy s logem Windows + R otevřete dialogové okno Spustit.

1. Napište wsreset.exe a zvolte **OK**.

1. Otevře se prázdné okno příkazového řádku. Po asi 10 sekundách se okno zavře a Microsoft Store se automaticky otevře.

**Krok 3: Resetujte službu Windows Update**

1. Vyberte **Start** > **Nastavení** > **Aktualizace a zabezpečení** > **Řešení potíží**.

1. Posuňte se dolů a ze seznamu vyberte **Služba Windows Update**, pak zvolte **Spustit poradce při potížích**.

1. Restartujte počítač a zkontrolujte, jestli pořád dochází k potížím.

