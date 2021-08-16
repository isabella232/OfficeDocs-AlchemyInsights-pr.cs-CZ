---
title: Více objektů má stejnou e-mailovou adresu jako identita.
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
ms.openlocfilehash: 5866d182cb2e97e37bc6df87e05fb6ef55bfed1d36f9daa95b7b8993a509e2dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011905"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Více objektů má stejnou e-mailovou adresu jako identita.

**Více objektů**

Jedním z běžných důvodů této chyby je, že není možné správně směrovat žádost Outlook Web Accessu za přítomnosti více objektů se stejnou e-mailovou adresou jako identita. Pokud chcete tyto objekty najít, spusťte následující příkazy:

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

Pokud chcete tento problém vyřešit, odeberte více objektů se stejnou identitou e-mailu a ujistěte se, že existuje jeden objekt s konkrétní identitou e-mailu a že jeho typem příjemce je UserMailbox.

**Stejná adresa se používá pro firemní a spotřebitelské poštovní schránky.**

Další příčinou je, když se stejná adresa používá pro firemní a spotřebitelské poštovní schránky. V takovém případě musí uživatel změnit svůj primární alias příjemce, dokud Cafe tento scénář nepodporuje. Jedná se o trvalou chybu, která nezmizí bez zásahu.

Podrobnosti najdete v tématu [Změna e-mailové adresy nebo telefonního](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)čísla účtu Microsoft.