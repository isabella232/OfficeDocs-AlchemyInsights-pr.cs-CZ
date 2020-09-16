---
title: 1336 RecoverableItems je plná.
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
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741260"
---
# <a name="the-recoverable-items-folder-is-full"></a>Složka pro obnovitelnou položky je plná

U poštovních schránek Exchange Online je výchozí limit úložiště pro složku pro obnovitelnost položek 30 GB. Pokud je poštovní schránka umístěná na podržení soudního sporu, podržení eDiscovery nebo je přiřazená zásada uchovávání informací, automaticky se 100 zvýší limit úložiště pro složku pro obnovitelnou položky.

Když složka se obnovitelnou položkami dosáhne limitu úložiště, bude funkčnost poštovní schránky ovlivněna následujícími způsoby:

- Uživatel nemůže odstranit položky z poštovní schránky.

- Pomocník pro spravovanou složku nemůže odstranit položky na základě značky uchovávání informací nebo nastavení spravované složky.

- U poštovních schránek, které mají povoleno obnovení jedné položky nebo jsou blokovány, nedokáže proces ochrany stránky kopírováním na disk zachovat verze položek upravovaných uživatelem.

- V případě poštovních schránek s povoleným protokolováním auditu poštovní schránky nelze do podsložky prověřit položky ukládat žádné položky protokolu auditování poštovní schránky.

U poštovních schránek, které nejsou blokovány, můžou správci pomocí `Search-Mailbox -SearchDumpsterOnly -DeleteContent` příkazu v PowerShellu pro Exchange Online odstranit položky ve složce obnovitelnou položky. Další informace najdete v těchto tématech:

- [Hledání a odstraňování zpráv](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Hledání – poštovní schránka](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

U poštovních schránek, které jsou blokovány, musí správci odebrat držení před odstraněním položek ze složky pro obnovitelnou položky. Další informace najdete v článku [o blokování položek ve složce pro obnovitelnou položky v cloudových poštovních schránkách](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Aby se zabránilo tomu, že se složka pro obnovu položek zablokuje, můžou správci zvýšit limit úložiště složky prohledatelné položky pro blokované poštovní schránky a nastavit zásady uchovávání poštovní schránky, které přesunou položky ze složky prohledatelné položky do archivované poštovní schránky uživatele. Přečtěte si téma [zvýšení kvóty pro obnovitelnou položky pro blokované poštovní schránky](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
