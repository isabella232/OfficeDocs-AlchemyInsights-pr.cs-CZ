---
title: Soubory na vyžádání
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: e0ba83778179abefe3ac4fe3e8ab0303d65ad929
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47803562"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="1522a-102">Konfigurace souborů na vyžádání</span><span class="sxs-lookup"><span data-stu-id="1522a-102">Configure Files On-Demand</span></span>

<span data-ttu-id="1522a-103">Soubory na OneDrivu na vyžádání vám pomohou přistupovat ke všem souborům na OneDrivu, aniž byste je museli stahovat a používat v zařízení úložný prostor.</span><span class="sxs-lookup"><span data-stu-id="1522a-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="1522a-104">Konfigurace souborů na vyžádání na počítači:</span><span class="sxs-lookup"><span data-stu-id="1522a-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="1522a-105">V oznamovací oblasti hlavního panelu Windows vyberte bílou nebo modrou ikonu cloudu **OneDrive** .</span><span class="sxs-lookup"><span data-stu-id="1522a-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="1522a-106">Vyberte ikonu **Nastavení** ozubeného kola & > **Nastavení**.</span><span class="sxs-lookup"><span data-stu-id="1522a-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="1522a-107">Na kartě **Nastavení** vyberte **ukládat místo a stahovat soubory, jak je používáte** .</span><span class="sxs-lookup"><span data-stu-id="1522a-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="1522a-108">Můžete taky nakonfigurovat soubory na vyžádání pomocí registru.</span><span class="sxs-lookup"><span data-stu-id="1522a-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="1522a-109">Pokud toto nastavení zakážete, budou mít uživatelé Windows 10 stejné chování synchronizace jako uživatelé předchozích verzí Windows a nemůžou zapínat soubory na vyžádání.</span><span class="sxs-lookup"><span data-stu-id="1522a-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="1522a-110">Pokud toto nastavení nenakonfigurujete, uživatelé můžou zapnout nebo vypnout soubory.</span><span class="sxs-lookup"><span data-stu-id="1522a-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="1522a-111">Když tuto zásadu povolíte, nastavíte následující hodnotu klíče registru na 1.</span><span class="sxs-lookup"><span data-stu-id="1522a-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="1522a-112">Když tuto zásadu zakážete, nastaví se následující hodnota klíče registru na 0.</span><span class="sxs-lookup"><span data-stu-id="1522a-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="1522a-113">Pokud se možnost soubory na vyžádání nezobrazuje v nastavení, ujistěte se, že je služba filtr souborů cloudové aplikace Windows nastavená na hodnotu 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="1522a-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="1522a-114">Povolením této funkce nastavíte následující hodnotu klíče registru na 2.</span><span class="sxs-lookup"><span data-stu-id="1522a-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`