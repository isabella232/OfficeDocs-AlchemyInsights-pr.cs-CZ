---
title: DataProtection – BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768810"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="954fa-102">Povolení šifrování nástrojem BitLocker s Intune</span><span class="sxs-lookup"><span data-stu-id="954fa-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="954fa-103">K nastavení šifrování nástroje BitLocker pro zařízení s Windows můžete použít zásady Endpoint Protection v Intune.</span><span class="sxs-lookup"><span data-stu-id="954fa-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="954fa-104">Další informace najdete v článku [nastavení Windows 10 (a novější), které chrání zařízení pomocí Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="954fa-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="954fa-105">Uvědomte si, že mnoho novějších zařízení s Windows 10 podporuje automatické šifrování nástrojem BitLocker, které se spouští bez zásad MDM.</span><span class="sxs-lookup"><span data-stu-id="954fa-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="954fa-106">To může ovlivnit použití zásad v případě, že nejsou nastavené výchozí nastavení.</span><span class="sxs-lookup"><span data-stu-id="954fa-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="954fa-107">Další podrobnosti najdete v následujících nejčastějších dotazech.</span><span class="sxs-lookup"><span data-stu-id="954fa-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="954fa-108">Informace o řešení problémů s nástrojem BitLocker najdete v článku [odstraňování potíží se zásadami nástrojem BitLocker v Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="954fa-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="954fa-109">**Nejčastější dotazy**</span><span class="sxs-lookup"><span data-stu-id="954fa-109">**FAQ**</span></span>

<span data-ttu-id="954fa-110">Otázka: jaké edice Windows podporují šifrování zařízení pomocí zásad ochrany koncových bodů?</span><span class="sxs-lookup"><span data-stu-id="954fa-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="954fa-111">A: nastavení v Intune Endpoint Protection se implementuje pomocí [CSP nástroje BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="954fa-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="954fa-112">CSP nepodporují všechny edice nebo buildy Windows.</span><span class="sxs-lookup"><span data-stu-id="954fa-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="954fa-113">Otázka: Jak povolit nástroj BitLocker na zařízeních bez nutnosti interakce s koncovým uživatelem</span><span class="sxs-lookup"><span data-stu-id="954fa-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="954fa-114">A: za předpokladu, že jsou splněny potřebné předpoklady, je možné povolit nástroj BitLocker "tiché šifrování" prostřednictvím Intune.</span><span class="sxs-lookup"><span data-stu-id="954fa-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="954fa-115">Prohlédněte si podrobnosti o požadavcích na zařízení a příklady nastavení zásad pro povolení tichého šifrování v následujícím dokumentu: [bezobslužné zapnutí šifrování nástrojem BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="954fa-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="954fa-116">Otázka: Pokud je už zařízení šifrované pomocí nástroje BitLocker s použitím výchozího nastavení OS pro metodu šifrování a složitost šifrování (XTS-AES-128), budou se při použití zásad s jinými nastaveními automaticky spouštět nové šifrování jednotky s novými nastaveními?</span><span class="sxs-lookup"><span data-stu-id="954fa-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="954fa-117">Odpověď: Ne.</span><span class="sxs-lookup"><span data-stu-id="954fa-117">A: No.</span></span> <span data-ttu-id="954fa-118">Pokud chcete použít nové nastavení šifrování, musí být jednotka nejdřív dešifrovaná.</span><span class="sxs-lookup"><span data-stu-id="954fa-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="954fa-119">**Poznámka:** U zařízení, která jsou registrovaná s automatickým pilotem, se automatické šifrování, které by se při spuštění předplatného spustilo, neaktivuje, dokud se nevyhodnotí zásada Intune, která umožňuje použití nastavení založených na zásadách místo výchozích hodnot operačního systému.</span><span class="sxs-lookup"><span data-stu-id="954fa-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="954fa-120">Otázka: Pokud je zařízení zašifrované v důsledku použití zásad Intune, bude při odebrání této zásady dešifrováno.</span><span class="sxs-lookup"><span data-stu-id="954fa-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="954fa-121">A: odstranění zásad týkajících se šifrování nemá za následek dešifrování nakonfigurovaných disků.</span><span class="sxs-lookup"><span data-stu-id="954fa-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="954fa-122">Otázka: Proč nastavení zásad dodržování předpisů v Intune ukazuje, že zařízení nemá zapnutý nástroj BitLocker, i když je?</span><span class="sxs-lookup"><span data-stu-id="954fa-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="954fa-123">A: nastavení "BitLocker Enabled" v zásadách dodržování předpisů Intune využívá klienta ověření stavu zařízení s Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="954fa-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="954fa-124">Tento klient měří pouze stav zařízení při spuštění.</span><span class="sxs-lookup"><span data-stu-id="954fa-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="954fa-125">Takže pokud se zařízení nerestartoval po dokončení šifrování nástrojem BitLocker, klientská služba nebude nástroj BitLocker ohlásit jako aktivní.</span><span class="sxs-lookup"><span data-stu-id="954fa-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 