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
ms.openlocfilehash: 10efdb5e1a90b3e279b8e1716e66a544d0ee34465245f5670930d8a9364a8cc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53977434"
---
# <a name="configure-files-on-demand"></a>Konfigurace souborů na vyžádání

OneDrive Soubory na vyžádání vyžadují [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (verze 1709 nebo novější) nebo Windows Server 2019 a OneDrive build 17.3.7064.1005 nebo novější.

OneDrive Soubory na vyžádání vám pomáhnou získat přístup ke všem souborům v OneDrive, aniž byste museli stahovat všechny soubory a používat úložný prostor na vašem zařízení.

Konfigurace souborů na vyžádání na počítači:

1. Na hlavním panelu OneDrive **na** hlavním panelu vyberte ikonu Windows nebo modré oznamovací oblast. Vyberte **ikonu nápověda & Nastavení** ozubeného kola > **Nastavení**.
2. Na kartě **Nastavení** vyberte pole Uložit místo a stahovat soubory **při jejich používání.**  

Soubory na vyžádání můžete taky nakonfigurovat pomocí registru.

Pokud toto nastavení zakážete, Windows 10 uživatelé mají stejné chování synchronizace jako uživatelé předchozích verzí Windows a nebudou moct zapnout možnost Soubory na vyžádání. Pokud toto nastavení nenakonfigurujete, mohou uživatelé zapnout nebo vypnout možnost Soubory na vyžádání.

Povolením této zásady nastavíte následující hodnotu klíče registru na hodnotu 1. Zakázáním této zásady nastavíte následující hodnotu klíče registru na hodnotu 0.

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

Pokud možnost Soubory na vyžádání nevidíte v Nastavení, ujistěte se, že typ startu "Windows Cloud Files Filter Driver" je nastavený na 2 (AUTO_START). Povolením této funkce nastavíte následující hodnotu klíče registru na hodnotu 2.

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`