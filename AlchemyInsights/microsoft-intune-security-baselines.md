---
title: Použití Microsoft Intune standardních hodnot zabezpečení ke konfiguraci Windows 10 zařízení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793614"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="e5c93-102">Použití Microsoft Intune standardních hodnot zabezpečení ke konfiguraci Windows 10 zařízení</span><span class="sxs-lookup"><span data-stu-id="e5c93-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="e5c93-103">Standardní hodnoty zabezpečení Intune pomáhají chránit uživatele a zařízení.</span><span class="sxs-lookup"><span data-stu-id="e5c93-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="e5c93-104">Standardní hodnoty zabezpečení Windows předkonfigurovaných skupin používaných k použití známé skupiny nastavení a výchozích hodnot doporučených příslušnými týmy zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="e5c93-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="e5c93-105">Vytvořením standardního profilu zabezpečení v Intune vytvoříte šablonu, která se skládá z více profilů konfigurace zařízení.</span><span class="sxs-lookup"><span data-stu-id="e5c93-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="e5c93-106">Když nasadíte standardní hodnoty zabezpečení do skupin uživatelů nebo zařízení, použije se nastavení na zařízeních, která běží na Windows 10 nebo novějších zařízeních.</span><span class="sxs-lookup"><span data-stu-id="e5c93-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="e5c93-107">Směrný plán zabezpečení mdm (Microsoft Mobile Device Management) například automaticky povolí nástroj BitLocker vyměnitelných jednotek, vyžaduje heslo pro odemknutí zařízení a zakáže základní ověřování.</span><span class="sxs-lookup"><span data-stu-id="e5c93-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="e5c93-108">Pokud výchozí hodnota pro vaše prostředí nefunguje, můžete přizpůsobit směrný plán tak, aby se na vás šoustá nastavení, která potřebujete.</span><span class="sxs-lookup"><span data-stu-id="e5c93-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="e5c93-109">Standardní hodnoty zabezpečení také pomáhají vytvořit zabezpečený pracovní postup mezi koncovými Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e5c93-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="e5c93-110">Směrný plán zabezpečení obsahuje doporučené postupy a doporučení pro nastavení, která mají vliv na zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="e5c93-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="e5c93-111">Intune spolupracuje s týmem Windows zabezpečení, který vytváří směrné plány pro zásady skupiny, takže tato doporučení jsou založená na solidní pokyny a rozsáhlém prostředí.</span><span class="sxs-lookup"><span data-stu-id="e5c93-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="e5c93-112">Pokud intune ještě nevíte, kde začít, standardní hodnoty zabezpečení vám pomůžou rychle vytvořit a nasadit zabezpečený profil.</span><span class="sxs-lookup"><span data-stu-id="e5c93-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="e5c93-113">Pokud aktuálně používáte zásady skupiny, migrace do Intune pro účely správy je mnohem jednodušší díky standardním hodnotám zabezpečení, protože jsou integrované do Intune a zahrnují špičkové možnosti správy.</span><span class="sxs-lookup"><span data-stu-id="e5c93-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="e5c93-114">Další informace najdete v článku [Windows standardních hodnot zabezpečení](/windows/security/threat-protection/windows-security-baselines) a správy [mobilních zařízení](/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="e5c93-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

