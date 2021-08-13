---
title: 1336 RecoverableItems folder is full
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061749"
---
# <a name="the-recoverable-items-folder-is-full"></a>Složka Obnovitelné položky je zaplněná.

U Exchange Online poštovních schránek je výchozí limit úložiště pro složku Obnovitelné položky 30 GB. Limit úložiště pro složku Obnovitelné položky se automaticky zvýší na 100 GB, pokud je poštovní schránka umístěná na blokování z důvodu soudního sporu, blokování eDiscovery nebo je přiřazená zásadám uchovávání informací.

Když složka Obnovitelné položky dosáhne limitu úložiště, bude funkce poštovní schránky ovlivněna následujícími způsoby:

- Uživatel nemůže odstranit položky z poštovní schránky.

- Pomocník pro spravované složky nemůže odstranit položky na základě značky uchovávání informací nebo nastavení spravované složky.

- U poštovních schránek, které mají povolené nebo blokované obnovení jedné položky, nemůže proces ochrany stránky při zápisu udržovat verze položek upravovaných uživatelem.

- U poštovních schránek s povoleným protokolováním auditování poštovní schránky se do podsložky Audity ve složce Obnovitelné položky nesloží žádné položky protokolu auditování poštovní schránky.

U poštovních schránek, které nejsou přidržené, mohou správci pomocí příkazu Exchange Online PowerShellu odstranit položky ve složce `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Obnovitelné položky. Další informace najdete v těchto tématech:

- [Hledání a odstraňování zpráv](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Hledání v poštovní schránce](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

U poštovních schránek, které jsou přidržené, musí správci blokování odebrat, aby mohli odstranit položky ze složky Obnovitelné položky. Další informace najdete v tématu Odstranění položek ve složce Obnovitelné položky [cloudových poštovních schránek](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)při blokování .

Aby se zabránilo zaplnění složky Obnovitelné položky, můžou správci zvýšit limit úložiště složky Obnovitelné položky pro poštovní schránky v blokování a nastavit zásadu uchovávání poštovních schránek, která přesune položky ze složky Obnovitelné položky do archivační poštovní schránky uživatele. Další informace najdete v článku Zvýšení kvóty obnovitelné položky [pro blokování poštovních schránek.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
