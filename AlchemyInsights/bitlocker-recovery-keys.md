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
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505061"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="1815f-102">Přístup k obnovovacím klíčům nástroje BitLocker</span><span class="sxs-lookup"><span data-stu-id="1815f-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="1815f-103">Při konfiguraci nastavení nástroje Bitlocker Intune Endpoint Protection Policy je možné definovat, jestli mají být informace o obnovení nástroje Bitlocker uložené ve službě Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1815f-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="1815f-104">Pokud je toto nastavení nakonfigurované, uložená data pro obnovení by měla být viditelná správci Intune jako součást dat záznamu zařízení v okně Zařízení Intune dvěma způsoby:</span><span class="sxs-lookup"><span data-stu-id="1815f-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="1815f-105">Zařízení – zařízení Azure AD –> zařízení nebo zařízení –> všechna zařízení –> "zařízení" –> obnovovací klíče</span><span class="sxs-lookup"><span data-stu-id="1815f-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="1815f-106">Pokud je k samotnému zařízení přístup pro správu, zobrazí se obnovovací klíč (Heslo) spuštěním následujícího příkazu z příkazového řádku se zvýšenými oprávněními:</span><span class="sxs-lookup"><span data-stu-id="1815f-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="1815f-107">Pokud bylo zařízení před přihlášením do Intune zašifrované, je možné, že byl obnovovací klíč přidružený k účtu Microsoft (MSA), který se používal k přihlášení k zařízení během procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="1815f-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="1815f-108">Pokud tomu tak bylo, měl by přístup k této službě msa a přihlášení se k této službě zobrazit zařízení,  https://onedrive.live.com/recoverykey pro která byly uložené obnovovací klíče.</span><span class="sxs-lookup"><span data-stu-id="1815f-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="1815f-109">Pokud bylo zařízení zašifrované v důsledku konfigurace prostřednictvím zásad skupiny založené na doméně, mohou být informace o obnovení uložené v místní službě Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1815f-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="1815f-110">Pokud jste nakonfigurovali zásady ochrany koncových bodů tak, aby se obnovovací klíč ukládal do Azure Active Directory, ale klíč pro konkrétní zařízení nebyl nahrán, můžete nahrávání spustit otočením obnovovací klávesy pro toto zařízení z konzoly MEM.</span><span class="sxs-lookup"><span data-stu-id="1815f-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="1815f-111">Podrobnosti najdete v tématu [Otočení obnovovacích klíčů nástroje BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="1815f-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

