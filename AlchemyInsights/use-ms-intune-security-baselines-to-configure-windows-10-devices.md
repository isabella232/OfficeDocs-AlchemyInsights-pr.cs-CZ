---
title: Konfigurace zařízení s Windows 10 pomocí standardních hodnot zabezpečení Microsoft Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573332"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="09757-102">Konfigurace zařízení s Windows 10 pomocí standardních hodnot zabezpečení Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="09757-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="09757-103">Plány zabezpečení Intune pomáhají chránit uživatele a zařízení.</span><span class="sxs-lookup"><span data-stu-id="09757-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="09757-104">Směrné plány zabezpečení: nastavení systému Windows – předdefinované skupiny používané k použití známé skupiny nastavení a výchozích hodnot doporučených příslušnými týmy zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="09757-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="09757-105">Vytvořením profilu zabezpečení podle směrného plánu v Intune vytvoříte šablonu, která se skládá z více konfiguračních profilů zařízení.</span><span class="sxs-lookup"><span data-stu-id="09757-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="09757-106">Při nasazení standardních hodnot zabezpečení do skupin uživatelů nebo zařízení se nastavení aplikuje na zařízení, která běží ve Windows 10 nebo novějším.</span><span class="sxs-lookup"><span data-stu-id="09757-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="09757-107">Například automatické přizpůsobení úrovně zabezpečení MDM (1) umožňuje BitLocker pro vyměnitelné jednotky (2) vyžaduje heslo pro odemknutí zařízení a (3) zakáže základní ověřování.</span><span class="sxs-lookup"><span data-stu-id="09757-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="09757-108">Pokud ve vašem prostředí nefunguje výchozí hodnota, upravte podle směrného plánu požadované nastavení.</span><span class="sxs-lookup"><span data-stu-id="09757-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="09757-109">Směrné plány zabezpečení pomáhají také při vytvoření zabezpečeného pracovního postupu v Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="09757-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="09757-110">Tady jsou některé výhody:</span><span class="sxs-lookup"><span data-stu-id="09757-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="09757-111">Směrný plán zabezpečení obsahuje osvědčené postupy a doporučení pro nastavení, která ovlivňují zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="09757-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="09757-112">Vzhledem k tomu, že partneři Intune se skupinou zabezpečení systému Windows, které vytvářejí směrné plány pro zásady skupiny, tato doporučení vycházejí z plných pokynů a rozsáhlých zkušeností.</span><span class="sxs-lookup"><span data-stu-id="09757-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="09757-113">Pokud se chystáte s Intune a nejste si jistí, kde začít, pak vám směrné plány zabezpečení umožní rychle vytvořit a nasadit zabezpečený profil.</span><span class="sxs-lookup"><span data-stu-id="09757-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="09757-114">Pokud v současné době používáte zásady skupiny, je migrace na Intune pro účely správy mnohem snadnější díky základním hodnotám zabezpečení, protože jsou integrované do Intune a zahrnují pro správu možnosti vyjímání.</span><span class="sxs-lookup"><span data-stu-id="09757-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="09757-115">Další informace najdete v tématu [směrné plány zabezpečení Windows](https://go.microsoft.com/fwlink/?linkid=2141503) a [Správa mobilních zařízení](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="09757-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>