---
title: Používání e-mailových profilů v Intune
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
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919416"
---
# <a name="using-email-profiles-with-intune"></a>Používání e-mailových profilů v Intune

Intune se používá k vytváření a nasazování e-mailových profilů pro nativního (integrovaného) e-mailového klienta na různých platformách zařízení.

Informace o některých omezeních souvisejících s e-mailovým profilem, včetně způsobu zpracování stavu existujících profilů a odebrání e-mailových profilů, najdete v tématu Přidání nastavení e-mailu do zařízení [pomocí Intune](https://docs.microsoft.com/intune/email-settings-configure).

Další informace o tom, jak vytvořit e-mailové profily pro každou platformu zařízení, najdete v těchto článku:

[Nastavení zařízení s Androidem pro konfiguraci e-mailu, ověřování a synchronizace v Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Přidání nastavení e-mailu pro zařízení s iOS a iPadOS v Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Nastavení profilu e-mailu v Microsoft Intune pro zařízení s Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Nastavení profilu e-mailu pro zařízení s Windows 10 v Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Běžný problém se synchronizací**

**E-mailový profil KNOX v Androidu zabraňuje synchronizaci kontaktů, kalendáře a úkolů uživatelů s uživatelskými zařízeními.**

E-mailový profil KNOX pro Android KNOX nabízí správci možnost rozhodnout se, které typy obsahu se mají synchronizovat se zařízením tak, že je nastavíte na povolené.

Pokud je nastavení pro některý z  typů obsahu nastavené na Nenakonfigurované (výchozí), nebude se tento typ obsahu synchronizovat automaticky. Uživatel může typ obsahu, který chce, povolit přímo na zařízení ručně, ale tato konfigurace se přepsána nastavením zásad Intune a synchronizace se zastaví pro tento typ obsahu.

