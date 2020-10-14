---
title: Veřejná složka s povoleným odesíláním pošty v EXO
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
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/13/2020
ms.locfileid: "48461781"
---
# <a name="sendas-mail-enabled-public-folder"></a>Veřejná složka s povoleným SendAs poštou

Následující příklad přiřadí oprávnění Odeslat jako pro veřejnou e-mailovou složku NewPF1 pro uživatele Jason.

Add-RecipientPermission-identity ' NewPF1 ' (důvěryhodný) "Jason"-AccessRights "SendAs"

Podrobné informace o syntaxi a parametrech najdete v tématu [přiřazení oprávnění "Odeslat jako" nebo "posílat v zastoupení jiné osoby" pro veřejné poštovní složky](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).

