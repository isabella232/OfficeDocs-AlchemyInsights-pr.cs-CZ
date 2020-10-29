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
# <a name="configure-files-on-demand"></a>Konfigurace souborů na vyžádání

Soubory na OneDrivu na vyžádání vyžadují [Windows 10 pro tvůrci aktualizací](https://go.microsoft.com/fwlink/p/?linkid=859040) (verze 1709 nebo novější) nebo windows server 2019 a OneDrive Build 17.3.7064.1005 nebo novější.

Soubory na OneDrivu na vyžádání vám pomohou přistupovat ke všem souborům na OneDrivu, aniž byste je museli stahovat a používat v zařízení úložný prostor.

Konfigurace souborů na vyžádání na počítači:

1. V oznamovací oblasti hlavního panelu Windows vyberte bílou nebo modrou ikonu cloudu **OneDrive** . Vyberte ikonu **Nastavení** ozubeného kola & > **Nastavení** .
2. Na kartě **Nastavení** vyberte **ukládat místo a stahovat soubory, jak je používáte** .  

Můžete taky nakonfigurovat soubory na vyžádání pomocí registru.

Pokud toto nastavení zakážete, budou mít uživatelé Windows 10 stejné chování synchronizace jako uživatelé předchozích verzí Windows a nemůžou zapínat soubory na vyžádání. Pokud toto nastavení nenakonfigurujete, uživatelé můžou zapnout nebo vypnout soubory.

Když tuto zásadu povolíte, nastavíte následující hodnotu klíče registru na 1. Když tuto zásadu zakážete, nastaví se následující hodnota klíče registru na 0.

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

Pokud se možnost soubory na vyžádání nezobrazuje v nastavení, ujistěte se, že je služba filtr souborů cloudové aplikace Windows nastavená na hodnotu 2 (AUTO_START). Povolením této funkce nastavíte následující hodnotu klíče registru na 2.

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`