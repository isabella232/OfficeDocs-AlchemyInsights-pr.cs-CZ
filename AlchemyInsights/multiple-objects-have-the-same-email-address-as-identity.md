---
title: Více objektů má stejnou e-mailovou adresu jako identita
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438800"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Více objektů má stejnou e-mailovou adresu jako identita

**Více objektů**

Jedním z běžných důvodů této chyby není možnost správně směrovat požadavek aplikace Outlook Web Access v přítomnosti více objektů, které mají stejnou e-mailovou adresu jako identita. Chcete-li tyto objekty najít, spusťte následující příkazy:

· Příjemce<email address>

· Získat uživatele<email address>

· Get-User <email address> -SoftDeleteduser

· Získat kontakt<email address>

· Poštovní <email address> schránka -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -NeaktivníMailboxOnly

Chcete-li tento problém vyřešit, odeberte více objektů se stejnou identitou e-mailu a ujistěte se, že existuje jeden objekt s konkrétní identitou e-mailu a že jeho typ příjemce je UserMailbox.

**Stejná adresa se používá pro obchodní a spotřebitelské poštovní schránky**

Další příčinou je, když se stejná adresa používá pro obchodní a spotřebitelské poštovní schránky. V takovém případě musí uživatel změnit svůj primární prostředek příjemce alias, dokud Kavárna podporuje tento scénář. Jedná se o trvalou chybu, která nezmizí bez zásahu.

Podrobnosti najdete [v tématu Změna e-mailové adresy nebo telefonního čísla účtu Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).