---
title: Podmínky chybějící v úložišti termínů SharePointu Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750444"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="77b49-102">Povolení šifrování nástrojem BitLocker s Intune</span><span class="sxs-lookup"><span data-stu-id="77b49-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="77b49-103">Zásady Endpoint Protection pro Intune se dají použít ke konfiguraci nastavení šifrování Boitlocker pro zařízení s Windows, jak je popsáno v: Windows10 (a novější) nastavení ochrany zařízení pomocí Intune.</span><span class="sxs-lookup"><span data-stu-id="77b49-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="77b49-104">Uvědomte si, že mnoho novějších zařízení s Windows 10 podporuje automatické šifrování BitLocker, které se spouští bez zásad MDM.</span><span class="sxs-lookup"><span data-stu-id="77b49-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="77b49-105">To může ovlivnit použití zásad, pokud nejsou konfigurovány výchozí nastavení.</span><span class="sxs-lookup"><span data-stu-id="77b49-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="77b49-106">Další podrobnosti najdete v častých otázkách.</span><span class="sxs-lookup"><span data-stu-id="77b49-106">See FAQ for more detail.</span></span>


<span data-ttu-id="77b49-107">Časté otázky   Q: jaké edice Windows podporují šifrování zařízení pomocí zásad ochrany koncových bodů?</span><span class="sxs-lookup"><span data-stu-id="77b49-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="77b49-108"> A: nastavení v Intune Endpoint Protection se implementuje pomocí CSP nástroje BitLocker.</span><span class="sxs-lookup"><span data-stu-id="77b49-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="77b49-109">CSP nepodporují všechny edice ani buildy Windows. 
     </span><span class="sxs-lookup"><span data-stu-id="77b49-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="77b49-110">Edice Windows: Enterprise; Podporují se vzdělávací, mobilní, mobilní a profesionální organizace (ze buildu 1809.</span><span class="sxs-lookup"><span data-stu-id="77b49-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="77b49-111">Otázka: Pokud je už zařízení zašifrované pomocí nástroje BitLocker s použitím výchozího nastavení OS pro metodu šifrování a šifrování (XTS-AES-128), bude se automaticky spouštět opětovné šifrování jednotky s novými nastaveními?</span><span class="sxs-lookup"><span data-stu-id="77b49-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="77b49-112">Odpověď: Ne.</span><span class="sxs-lookup"><span data-stu-id="77b49-112">A: No.</span></span> <span data-ttu-id="77b49-113">Pokud chcete použít nové nastavení šifrování, musí být jednotka nejdřív dešifrovaná.</span><span class="sxs-lookup"><span data-stu-id="77b49-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="77b49-114">Poznámka: u zařízení, která jsou registrovaná pomocí automatického pilotního nasazení, se automatické šifrování, ke kterému dojde při vyhodnocování zásad při spuštění, neaktivuje, dokud neproběhne vyhodnocení zásady Intune, která umožňuje použití nastavení založených na zásadách místo výchozích hodnot operačního systému.</span><span class="sxs-lookup"><span data-stu-id="77b49-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="77b49-115">Otázka Pokud je zařízení zašifrované v důsledku použití zásad Intune, bude při odebrání této zásady dešifrováno?</span><span class="sxs-lookup"><span data-stu-id="77b49-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="77b49-116">A: odebrání zásad souvisejících se šifrováním nemá za následek dešifrování nakonfigurovaných disků.</span><span class="sxs-lookup"><span data-stu-id="77b49-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="77b49-117">Otázka: Proč zásady pro dodržování předpisů v Intune ukazují, že moje zařízení nemá povolený nástroj BitLocker, ale je?</span><span class="sxs-lookup"><span data-stu-id="77b49-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="77b49-118">A: nastavení "BitLocker Enabled" v zásadách dodržování předpisů Intune využívá klienta ověření stavu zařízení s Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="77b49-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="77b49-119">Tento klient měří pouze stav zařízení při spuštění.</span><span class="sxs-lookup"><span data-stu-id="77b49-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="77b49-120">Takže pokud se zařízení nerestartoval po dokončení šifrování nástrojem BitLocker, klientská služba nebude nástroj BitLocker ohlásit jako aktivní.</span><span class="sxs-lookup"><span data-stu-id="77b49-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>