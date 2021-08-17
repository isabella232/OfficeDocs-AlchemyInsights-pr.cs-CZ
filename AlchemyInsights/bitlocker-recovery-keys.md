---
title: Obnovovací klíče nástroje BitLocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060057"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Přístup k obnovovacím klíčům nástroje BitLocker

Při konfiguraci nastavení nástroje Bitlocker Endpoint Protection Intune zásady, je možné definovat, jestli mají být informace o obnovení nástroje Bitlocker uložené v Azure Active Directory.

Pokud je toto nastavení nakonfigurované, uložená data pro obnovení by měla být viditelná správci Intune jako součást dat záznamu zařízení v okně Zařízení Intune dvěma způsoby:

Zařízení – zařízení Azure AD –> zařízení nebo zařízení –> všechna zařízení –> "zařízení" –> obnovovací klíče

Pokud je k samotnému zařízení přístup pro správu, zobrazí se obnovovací klíč (Heslo) spuštěním následujícího příkazu z příkazového řádku se zvýšenými oprávněními:

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
Pokud bylo zařízení před přihlášením do Intune zašifrované, je možné, že byl obnovovací klíč přidružený k účtu Microsoft (MSA), který se používal k přihlášení k zařízení během procesu OOBE. Pokud tomu tak bylo, měl by přístup k této službě msa a přihlášení se k této službě zobrazit zařízení,  https://onedrive.live.com/recoverykey pro která byly uložené obnovovací klíče.
 
Pokud bylo zařízení zašifrované v důsledku konfigurace prostřednictvím zásad skupiny založené na doméně, mohou být informace o obnovení uložené v místní službě Active Directory.

Pokud jste nakonfigurovali zásady ochrany koncových bodů tak, aby se obnovovací klíč ukládal do Azure Active Directory ale klíč pro konkrétní zařízení nebyl nahrán, můžete nahrávání spustit otočením obnovovací klávesy pro toto zařízení z konzoly MEM. Podrobnosti najdete v tématu [Otočení obnovovacích klíčů nástroje BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

