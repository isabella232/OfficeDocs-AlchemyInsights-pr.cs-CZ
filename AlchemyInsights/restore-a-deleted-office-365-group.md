---
title: Obnovení odstraněné Microsoft 365 skupiny
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959019"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Obnovení odstraněné Microsoft 365 skupiny

Odstraněnou skupinu Microsoft 365 nebo Microsoft Teams obnovit do 30 dnů od odstranění.

1. Přejděte na [Centrum pro správu Microsoftu 365](https://aka.ms/RestoreDeletedGroup) a přihlaste se k seznamu odstraněných skupin a týmů.

    **Poznámka:** Přihlaste se pomocí účtu, který je přiřazený správci tenanta nebo roli správce skupin.

1. Vyberte odstraněnou skupinu Microsoft 365 nebo Teams, která se má obnovit, a klikněte **na obnovit skupinu.**

    Pokud skupinu nemůžete obnovit kvůli konfliktní adrese SMTP, použijte následující příkaz k vyhledání objektu, který způsobuje konflikt, a odeberte adresu SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Poznámka:** V některých případech může trvat až 24 hodin, než se skupina a všechna její data obnoví.

    Další informace nebo se dozvíte, jak obnovit skupiny pomocí PowerShellu, najdete v článku Obnovení [odstraněné Microsoft 365 skupiny.](https://go.microsoft.com/fwlink/?linkid=867802)