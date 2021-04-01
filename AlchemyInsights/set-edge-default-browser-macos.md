---
title: Nastavení Microsoft Edge jako výchozího prohlížeče na zařízení s macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491361"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="e3c2e-102">Nastavení Microsoft Edge jako výchozího prohlížeče na zařízení s macOS</span><span class="sxs-lookup"><span data-stu-id="e3c2e-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="e3c2e-103">K nastavení Microsoft Edge jako výchozího prohlížeče použijte jednu z těchto dvou metod:</span><span class="sxs-lookup"><span data-stu-id="e3c2e-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="e3c2e-104">Metoda 1: Flash zařízení s obrázkem macOS, kde microsoft edge už byl nastavený jako výchozí prohlížeč.</span><span class="sxs-lookup"><span data-stu-id="e3c2e-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="e3c2e-105">Metoda 2: Nastavte zásadu DefaultBrowserSettingEnabled tak, aby vyzvat uživatele, aby nastavil Microsoft Edge jako výchozí prohlížeč.</span><span class="sxs-lookup"><span data-stu-id="e3c2e-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="e3c2e-106">Obě metody umožňují uživateli změnit výchozí prohlížeč.</span><span class="sxs-lookup"><span data-stu-id="e3c2e-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="e3c2e-107">Z tohoto důvodu doporučujeme nasadit zásadu DefaultBrowserSettingEnabled, i když jste použili metodu 1.</span><span class="sxs-lookup"><span data-stu-id="e3c2e-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="e3c2e-108">Pokud uživatel po nasazení zásady změní výchozí prohlížeč, zobrazí se v zásadách výzva k nastavení výchozího prohlížeče zpátky na Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="e3c2e-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
