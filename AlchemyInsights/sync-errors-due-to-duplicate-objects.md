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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708055"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Chyby synchronizace kvůli duplicitním objektům

Po dokončení synchronizace adresářů v Microsoftu 365 se může zobrazit jedna z následujících chybových zpráv:

- Tento objekt nelze aktualizovat ve službách Microsoft Online Services, protože následující atributy přidružené k tomuto objektu mají hodnoty, které mohou být již přidruženy k jinému objektu v místním adresáři.

- Synchronizovaný objekt se stejnou adresou proxy serveru už v adresáři služeb Microsoft Online Services existuje.

- Tento objekt nelze aktualizovat, protože následující atributy přidružené k tomuto objektu mají hodnoty, které již mohou být přidruženy k jinému objektu v místních adresářových službách: UserPrincipalName.

Pokud chcete tento problém identifikovat a opravit, stáhněte a spusťte Nástroj [IdFix DirSync Error Remediation Tool.](https://github.com/Microsoft/idfix)

Další informace najdete v [článku KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
