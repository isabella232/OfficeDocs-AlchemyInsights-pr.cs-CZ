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
ms.openlocfilehash: 4e3da81ee048c6257e05b998c0f457fa433738fd
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791287"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="a5959-102">Konfigurace souborů na vyžádání</span><span class="sxs-lookup"><span data-stu-id="a5959-102">Configure Files On-Demand</span></span>

<span data-ttu-id="a5959-103">Soubory na OneDrivu na vyžádání vyžadují [Windows 10 pro tvůrci aktualizací](https://go.microsoft.com/fwlink/p/?linkid=859040) (verze 1709 nebo novější) nebo windows server 2019 a OneDrive Build 17.3.7064.1005 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="a5959-103">OneDrive Files On-Demand requires [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (version 1709 or later) or Windows Server 2019 and OneDrive build 17.3.7064.1005 or later.</span></span>

<span data-ttu-id="a5959-104">Soubory na OneDrivu na vyžádání vám pomohou přistupovat ke všem souborům na OneDrivu, aniž byste je museli stahovat a používat v zařízení úložný prostor.</span><span class="sxs-lookup"><span data-stu-id="a5959-104">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="a5959-105">Konfigurace souborů na vyžádání na počítači:</span><span class="sxs-lookup"><span data-stu-id="a5959-105">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="a5959-106">V oznamovací oblasti hlavního panelu Windows vyberte bílou nebo modrou ikonu cloudu **OneDrive** .</span><span class="sxs-lookup"><span data-stu-id="a5959-106">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="a5959-107">Vyberte ikonu **Nastavení** ozubeného kola & > **Nastavení** .</span><span class="sxs-lookup"><span data-stu-id="a5959-107">Select the **Help & Settings** gear icon > **Settings** .</span></span>
2. <span data-ttu-id="a5959-108">Na kartě **Nastavení** vyberte **ukládat místo a stahovat soubory, jak je používáte** .</span><span class="sxs-lookup"><span data-stu-id="a5959-108">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="a5959-109">Můžete taky nakonfigurovat soubory na vyžádání pomocí registru.</span><span class="sxs-lookup"><span data-stu-id="a5959-109">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="a5959-110">Pokud toto nastavení zakážete, budou mít uživatelé Windows 10 stejné chování synchronizace jako uživatelé předchozích verzí Windows a nemůžou zapínat soubory na vyžádání.</span><span class="sxs-lookup"><span data-stu-id="a5959-110">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="a5959-111">Pokud toto nastavení nenakonfigurujete, uživatelé můžou zapnout nebo vypnout soubory.</span><span class="sxs-lookup"><span data-stu-id="a5959-111">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="a5959-112">Když tuto zásadu povolíte, nastavíte následující hodnotu klíče registru na 1.</span><span class="sxs-lookup"><span data-stu-id="a5959-112">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="a5959-113">Když tuto zásadu zakážete, nastaví se následující hodnota klíče registru na 0.</span><span class="sxs-lookup"><span data-stu-id="a5959-113">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="a5959-114">Pokud se možnost soubory na vyžádání nezobrazuje v nastavení, ujistěte se, že je služba filtr souborů cloudové aplikace Windows nastavená na hodnotu 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="a5959-114">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="a5959-115">Povolením této funkce nastavíte následující hodnotu klíče registru na 2.</span><span class="sxs-lookup"><span data-stu-id="a5959-115">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`