---
title: Obnovovací klíče nástroje BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685879"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Přístup k obnovovacím klíčům nástroje BitLocker

Při konfiguraci zásad služby Endpoint Protection v nastavení BitLockeru je možné určit, zda mají být informace pro obnovení BitLocker uložené v Azure Active Directory.

Pokud je toto nastavení nakonfigurováno, budou se uložená data obnovení zobrazovat v Intune správci jako součást dat záznamu zařízení v okně v Intune

Zařízení – zařízení Azure AD – > zařízení nebo zařízení – > všechna zařízení – > "zařízení" – > klíče pro obnovení

Pokud máte k samotnému zařízení přístup pro správu, může se zobrazit obnovovací klíč (heslo) spuštěním následujícího příkazu z příkazového řádku s vyššími oprávněními:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Pokud bylo zařízení před enrolment v Intune zašifrované, mohlo by být obnovovací klíč přidružen k účtu Microsoft (MSA), který se používá k přihlášení na zařízení během procesu OOBE. V takovém případě  https://onedrive.live.com/recoverykey by měl přístup a přihlášení pomocí tohoto MSA zobrazovat zařízení, pro které byly uložené klíče obnovení.
 
Pokud bylo zařízení zašifrováno jako výsledek konfigurace prostřednictvím zásad skupiny domény, mohou být informace pro obnovení uloženy v místní službě Active Directory.
 

