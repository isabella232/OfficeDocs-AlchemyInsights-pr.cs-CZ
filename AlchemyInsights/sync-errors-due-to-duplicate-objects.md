---
title: 902 (chyby synchronizace kvůli duplicitním objektům)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737334"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Chyby synchronizace kvůli duplicitním objektům

Při dokončení synchronizace adresáře v Microsoft 365 se může zobrazit jedna z následujících chybových zpráv:

- Tento objekt nejde aktualizovat v online službách Microsoftu, protože následující atributy přidružené k tomuto objektu mají hodnoty, které už můžou být přidružené k jinému objektu v místním adresáři.

- Synchronizovaný objekt se stejnou proxy adresou už v adresáři služeb Microsoft Online Services existuje.

- Tento objekt nejde aktualizovat, protože následující atributy přidružené k tomuto objektu mají hodnoty, které už můžou být přidružené k jinému objektu v místních adresářových službách: UserPrincipalName.

Chcete-li zjistit a opravit problém, Stáhněte a spusťte [Nástroj IdFix DirSync chyby](https://www.microsoft.com/download/details.aspx?id=36832).

Další informace najdete v tématu [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
