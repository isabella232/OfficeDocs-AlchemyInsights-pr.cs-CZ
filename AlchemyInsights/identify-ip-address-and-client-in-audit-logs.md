---
title: Identifikace IP adresy a klienta v protokolech auditování
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668303"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifikace IP adresy a klienta v protokolech auditování

V protokolech auditování se zobrazuje IP adresa, která odpovídá aktivitě od uživatele Microsoft 365. Informace o klientovi jsou protokolovány také. Tady je postup, jak tyto informace zjistit.

1. Přihlaste se do [centra zabezpečení Microsoft 365 Security &](https://protection.office.com/).

2. Přejděte na stránku **Search**pro  >  **vyhledávání protokolu auditování** .

   Pokud máte zájem o konkrétní aktivitu, vyberte ji ze seznamu **aktivity** . Pokud ne, budou pro vybraného uživatele (výchozí nastavení) vráceny všechny aktivity.

   **Poznámka**: určité aktivity nemusí být dostupné v nabídce **aktivity** . Tyto položky auditu budou vráceny, pokud je vybrána možnost **Zobrazit výsledky pro všechny aktivity** (výchozí nastavení).

3. V poli **Uživatelé** zadejte uživatelské jméno, vyberte odpovídající rozsah kalendářních dat a klikněte na **Hledat**.

Ve výsledcích se zobrazí IP adresa této aktivity v podokně výsledků. Pokud chcete zobrazit podrobné informace v informačním panelu **podrobností** (například klient, uživatel, který provedl akci atd.), vyberte záznam auditování.

Další informace najdete v tématu [Vyhledání IP adresy počítače použitého pro přístup k ohroženému účtu](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
