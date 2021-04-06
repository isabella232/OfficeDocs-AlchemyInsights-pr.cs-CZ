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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597436"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Obnovení odstraněné skupiny Microsoft 365

Odstraněnou skupinu Microsoft 365 nebo Microsoft Teams můžete obnovit do 30 dnů od odstranění.

1. Přejděte do [Centra pro správu Microsoftu 365 a](https://aka.ms/RestoreDeletedGroup) přihlaste se a seznam odstraněných skupin a týmů.

    **Poznámka:** Přihlaste se pomocí účtu, který je přiřazený správci tenanta nebo roli správce skupin.

1. Vyberte odstraněnou skupinu Microsoft 365/Teams, která se má obnovit, a klikněte **na obnovit skupinu.**

    Pokud skupinu nemůžete obnovit kvůli konfliktní adrese SMTP, použijte následující příkaz k vyhledání objektu, který způsobuje konflikt, a odeberte adresu SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Poznámka:** V některých případech může trvat až 24 hodin, než se skupina a všechna její data obnoví.

    Další informace nebo informace o obnovení skupin pomocí PowerShellu najdete v tématu Obnovení odstraněné skupiny [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)