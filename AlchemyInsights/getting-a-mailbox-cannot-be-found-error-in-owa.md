---
title: 126 Při získání poštovní schránky se v aplikaci OWA nenašla chyba?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056483"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Chyba v poštovní schránce se v Outlook na webu?

Pokud používáte Outlook na webu **a** zobrazí se chyba Poštovní schránka, účet, který jste použili pro připojení k Outlook na webu, nemá licenci Exchange Online, a proto není k účtu přidružená žádná poštovní schránka. Správce může přiřadit licenci k vašemu účtu takto:

1. Otevřete [Centrum pro správu Microsoftu 365](https://portal.office.com/adminportal/home#/homepage) a v  části Uživatelé  přejděte na Aktivní uživatelé a vyberte uživatele, který chybu vidí.

2. Na stránce uživatele, která se  otevře, přejděte do části  Licence a aplikace, vyberte příslušnou hodnotu Umístění a přiřaďte licenci, která obsahuje Exchange Online (rozbalte licenci a zobrazte její podrobnosti). Až skončíte, klikněte na **Uložit změny**.

V některých případech, pokud je licence už přiřazená k uživatelskému účtu, pomáhá odebrání a opětovné přiřazení licence problém vyřešit a zajistit jeho správné zřízení v systému: 

- Zkontrolujte, jestli jsou vaše předplatná M365 Exchange Online (a další, pokud máte) aktuální a ještě nedávno nevyšly.

Po ověření, že platnost vašeho předplatného nevy vypršela a byla přiřazena platná licence k uživatelskému účtu, může zřízení licence trvat až 24 hodin, takže budete muset počkat, až se problém vyřeší. Další informace najdete v tématu [Přiřazení a správa licencí](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).