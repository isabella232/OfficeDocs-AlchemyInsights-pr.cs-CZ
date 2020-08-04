---
title: Používání e-mailových profilů s Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554843"
---
# <a name="using-email-profiles-with-intune"></a>Používání e-mailových profilů s Intune

Intune se dá použít k vytvoření a nasazení e-mailových profilů pro nativního (integrovaného) e-mailového klienta na platformách více zařízení.

Informace o některých omezeních spojených s e-mailovými profily, včetně způsobu zpracování stavu existujících profilů a odebrání e-mailových profilů, najdete v tématu [Přidání nastavení e-mailu do zařízení pomocí Intune](https://docs.microsoft.com/intune/email-settings-configure).

Další informace o vytváření e-mailových profilů pro jednotlivé platformy zařízení najdete v tématu:

[Nastavení zařízení Android pro konfiguraci e-mailu, ověřování a synchronizace v Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Přidání nastavení e-mailu pro zařízení s iOS a iPadOS v Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Nastavení e-mailového profilu v Microsoft Intune pro zařízení s Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Nastavení e-mailového profilu pro zařízení s Windows 10 v Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Běžný problém se synchronizací**

**E-mailový profil KNOX v systému Android zabraňuje synchronizaci kontaktů, kalendářů a úkolů uživatelů s uživatelskými zařízeními.**

E-mailový profil KNOX v systému Android KNOX nabízí správci možnost rozhodnout, které typy obsahu jsou synchronizovány se zařízením, a to tak, že každý z nich bude povolen.

Pokud je nastavení pro některý z typů obsahu nastaveno na **Možnost Není nakonfigurováno** (výchozí), tento typ obsahu se automaticky nesynchronizuje. Uživatel může povolit typ obsahu, který chce přímo na zařízení ručně, ale tato konfigurace je přepsána nastavením zásad Intune a synchronizace se zastaví pro tento typ obsahu.

