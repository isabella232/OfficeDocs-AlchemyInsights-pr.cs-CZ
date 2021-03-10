---
title: Použití standardních hodnot zabezpečení Microsoft Intune ke konfiguraci zařízení s Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50693416"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="a4526-102">Použití standardních hodnot zabezpečení služby Microsoft Intune při konfiguraci zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="a4526-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="a4526-103">Standardní hodnoty zabezpečení Intune pomáhají chránit uživatele a zařízení.</span><span class="sxs-lookup"><span data-stu-id="a4526-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="a4526-104">Směrné plány zabezpečení jsou předem nakonfigurované skupiny nastavení Windows používané k použití známé skupiny nastavení a výchozích hodnot doporučených příslušnými týmy zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="a4526-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="a4526-105">Vytvořením standardního profilu zabezpečení v Intune vytvoříte šablonu, která se skládá z více profilů konfigurace zařízení.</span><span class="sxs-lookup"><span data-stu-id="a4526-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="a4526-106">Když nasadíte standardní hodnoty zabezpečení pro skupiny uživatelů nebo zařízení, nastavení se použije na zařízeních s Windows 10 nebo novějších verzích.</span><span class="sxs-lookup"><span data-stu-id="a4526-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="a4526-107">Například standardní hodnoty zabezpečení MDM (Mobile Device Management) microsoftu automaticky (1) umožňují nástroji BitLocker použít vyměnitelné jednotky, (2) vyžaduje heslo k odemknutí zařízení a (3) zakáže základní ověřování.</span><span class="sxs-lookup"><span data-stu-id="a4526-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="a4526-108">Pokud ve vašem prostředí výchozí hodnota nefunguje, můžete přizpůsobit směrný plán a použít tak nastavení, která potřebujete.</span><span class="sxs-lookup"><span data-stu-id="a4526-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="a4526-109">Směrné plány zabezpečení taky pomáhají vytvořit v Microsoftu 365 zabezpečený pracovní postup od začátku do konce.</span><span class="sxs-lookup"><span data-stu-id="a4526-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="a4526-110">Některé výhody této funkce jsou následující:</span><span class="sxs-lookup"><span data-stu-id="a4526-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="a4526-111">Směrný plán zabezpečení zahrnuje doporučené postupy a doporučení pro nastavení, která mají vliv na zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="a4526-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="a4526-112">Protože Intune spolupracuje s týmem zabezpečení Windows, který vytváří standardní hodnoty pro zásady skupiny, jsou tato doporučení založená na solidní pokyny a rozsáhlém prostředí.</span><span class="sxs-lookup"><span data-stu-id="a4526-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="a4526-113">Pokud Intune ještě nevíte, kde začít, standardní hodnoty zabezpečení vám pomůžou rychle vytvořit a nasadit zabezpečený profil.</span><span class="sxs-lookup"><span data-stu-id="a4526-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="a4526-114">Pokud v současné době používáte zásady skupiny, je migrace na Intune pro účely správy mnohem jednodušší, protože tyto standardní hodnoty zabezpečení jsou integrované v Intune a zahrnují špičkové funkce pro správu.</span><span class="sxs-lookup"><span data-stu-id="a4526-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="a4526-115">Další informace najdete v [standardních hodnotách zabezpečení Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) [a správě mobilních zařízení.](https://docs.microsoft.com/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="a4526-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>