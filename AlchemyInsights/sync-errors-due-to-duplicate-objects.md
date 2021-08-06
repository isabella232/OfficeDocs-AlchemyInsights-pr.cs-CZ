---
title: 902 (Chyby synchronizace kvůli duplicitním objektům)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998778"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Chyby synchronizace způsobené duplicitními objekty

Po dokončení synchronizace adresářů se může zobrazit jedna z následujících chybových Microsoft 365:

- Tento objekt nelze aktualizovat ve službách Microsoft Online Services, protože následující atributy přidružené k tomuto objektu mají hodnoty, které už bývají přidružené k jinému objektu v místním adresáři.

- Synchronizovaný objekt se stejnou adresou proxy serveru už v adresáři služeb Microsoft Online Services existuje.

- Tento objekt nelze aktualizovat, protože následující atributy přidružené k tomuto objektu mají hodnoty, které už bývají přidružené k jinému objektu v místních adresářových službách: UserPrincipalName.

Pokud chcete tento problém identifikovat a vyřešit, stáhněte a spusťte nástroj [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).

Další informace najdete v [článku KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
