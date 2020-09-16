---
title: Používání profilů e-mailů s Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653281"
---
# <a name="using-email-profiles-with-intune"></a>Používání profilů e-mailů s Intune

Intune se dá použít k vytvoření a nasazení profilů e-mailů pro nativní (vestavěný) e-mailový klient na více platformách zařízení.

Informace o některých omezeních souvisejících s e-mailovými profily, včetně způsobu, jakým se řídí přítomnost stávajících profilů a jak odebrat profily e-mailu, najdete v článku [Přidání nastavení e-mailu do zařízení pomocí Intune](https://docs.microsoft.com/intune/email-settings-configure).

Další informace o vytváření profilů e-mailů pro jednotlivé platformy zařízení najdete v těchto tématech:

[Nastavení zařízení s Androidem pro konfiguraci e-mailů, ověřování a synchronizace v Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Přidání nastavení e-mailu pro zařízení s iOS a iPadOS v Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Nastavení e-mailového profilu v Microsoft Intune pro zařízení s Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Nastavení e-mailového profilu pro zařízení s Windows 10 v Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Běžný problém se synchronizací**

**V e-mailovém profilu pro Android brání uživatelům, kalendářům a úkolům v synchronizaci s uživatelskými zařízeními.**

V e-mailovém profilu pro Android KNOX nabízí správce možnost rozhodnout se, které typy obsahu se budou synchronizovat, nastavením příslušných možností.

Pokud je nastavení libovolného typu obsahu nastaveno na **Nenakonfigurováno** (výchozí nastavení), nebude tento typ obsahu automaticky synchronizován. Uživatel může povolit, aby typ obsahu, který mají být přímo v zařízení, byl v nastavení zásad Intune přepsán a synchronizace se u tohoto typu obsahu zastaví.

