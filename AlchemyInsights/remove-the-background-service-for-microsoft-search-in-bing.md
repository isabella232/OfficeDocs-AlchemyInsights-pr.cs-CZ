---
title: Odebrání služby pozadí pro Microsoft Search v Bingu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816091"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Odebrání služby pozadí pro Microsoft Search v Bingu

Pokud chcete odebrat službu pozadí pro Microsoft Search v Bingu, můžete vyzkoušet následující prostředky nápravy:

1. Pokud se chcete vrátit k původnímu nastavení vyhledávacího webu, proveďte následující kroky:

    a. Přepněte **přepínač Používat Bing jako výchozí vyhledávací [modul.](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**

    b. [Přejděte do Centra pro správu Microsoftu 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) a zrušte nastavení, které se týká všech uživatelů ve vaší organizaci.

2. Pokud chcete odebrat službu pozadí z jednotlivých zařízení, proveďte následující úkoly:

    a. Zvolte **Ovládací panely > Programy > Programy a funkce**.

    b. V seznamu nainstalovaných programů klikněte pravým tlačítkem myši na **Microsoft Search v Bingu** a potom klikněte na **Odinstalovat.**

3. Pokud chcete odebrat službu pozadí z více zařízení ve vaší organizaci, přihlaste se jako správce a ve skriptu spusťte následující příkaz: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
