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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="5c70a-102">Přístup k obnovovacím klíčům nástroje BitLocker</span><span class="sxs-lookup"><span data-stu-id="5c70a-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="5c70a-103">Při konfiguraci zásad služby Endpoint Protection v nastavení BitLockeru je možné určit, zda mají být informace pro obnovení BitLocker uložené v Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5c70a-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="5c70a-104">Pokud je toto nastavení nakonfigurováno, budou se uložená data obnovení zobrazovat v Intune správci jako součást dat záznamu zařízení v okně v Intune</span><span class="sxs-lookup"><span data-stu-id="5c70a-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="5c70a-105">Zařízení – zařízení Azure AD – > zařízení nebo zařízení – > všechna zařízení – > "zařízení" – > klíče pro obnovení</span><span class="sxs-lookup"><span data-stu-id="5c70a-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="5c70a-106">Pokud máte k samotnému zařízení přístup pro správu, může se zobrazit obnovovací klíč (heslo) spuštěním následujícího příkazu z příkazového řádku s vyššími oprávněními:</span><span class="sxs-lookup"><span data-stu-id="5c70a-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="5c70a-107">Pokud bylo zařízení před enrolment v Intune zašifrované, mohlo by být obnovovací klíč přidružen k účtu Microsoft (MSA), který se používá k přihlášení na zařízení během procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="5c70a-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="5c70a-108">V takovém případě  https://onedrive.live.com/recoverykey by měl přístup a přihlášení pomocí tohoto MSA zobrazovat zařízení, pro které byly uložené klíče obnovení.</span><span class="sxs-lookup"><span data-stu-id="5c70a-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="5c70a-109">Pokud bylo zařízení zašifrováno jako výsledek konfigurace prostřednictvím zásad skupiny domény, mohou být informace pro obnovení uloženy v místní službě Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5c70a-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

