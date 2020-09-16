---
title: Více objektů má stejnou e-mailovou adresu jako identita
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724608"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Více objektů má stejnou e-mailovou adresu jako identita

**Více objektů**

Jedním ze častých důvodů této chyby není umožnit správné směrování požadavku aplikace Outlook Web Access v přítomnosti více objektů se stejnou e-mailovou adresou jako identita. K vyhledání těchto objektů použijte následující příkazy:

· Get-příjemce <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Získat kontakt <email address>

· Get – poštovní schránka <email address> – PublicFolder

· Get – poštovní schránka <email address> – IncludeSoftDeletedMailbox

· Get – poštovní schránka <email address> – InactiveMailboxOnly

Tento problém vyřešíte tak, že odeberete více objektů se stejnou e-mailovou identitou a zajistěte, aby byl jediný objekt se specifickou identitou e-mailu a aby jeho typ příjemce byl UserMailbox.

**Pro firemní a spotřebitelské poštovní schránky se používá stejná adresa**

Další příčina je, když se pro firemní a spotřebitelské poštovní schránky používá stejná adresa. V tomto případě musí uživatel změnit svůj primární alias pro uživatele, dokud kavárny tento scénář nepodporuje. Jedná se o trvalou chybu, která není bez zásahu.

Podrobnosti najdete v článku [Změna e-mailové adresy nebo telefonního čísla pro váš účet Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).