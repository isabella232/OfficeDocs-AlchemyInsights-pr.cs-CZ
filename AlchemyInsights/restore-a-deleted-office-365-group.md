---
title: Obnovení odstraněné skupiny Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645124"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Obnovení odstraněné skupiny Microsoft 365

Odstraněnou skupinu Microsoft 365 nebo Microsoft Teams můžete obnovit do 30 dnů od odstranění.

1. Přejděte do [Centra pro správu Microsoftu 365](https://aka.ms/RestoreDeletedGroup) a přihlaste se k seznamu odstraněných skupin a týmů.

    **Poznámka:** Přihlaste se pomocí účtu, který je přiřazený správci tenanta nebo roli správce skupin.

1. Vyberte odstraněnou skupinu Microsoft 365/Teams, která se má obnovit, a klikněte **na obnovit skupinu.**

    Pokud skupinu nemůžete obnovit kvůli konfliktní adrese SMTP, použijte následující příkaz k vyhledání objektu, který způsobuje konflikt, a odeberte adresu SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Poznámka:** V některých případech může trvat až 24 hodin, než se skupina a všechna její data obnoví.

    Další informace nebo informace o obnovení skupin pomocí PowerShellu najdete v tématu Obnovení odstraněné skupiny [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)