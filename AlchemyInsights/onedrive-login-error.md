---
title: OneDrive přihlášení AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112905"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive přihlášení AADSTS50011

Pokud se zobrazí chybová zpráva "AADSTS50011: Adresa URL odpovědi zadaná v žádosti neodpovídá odpovědi" při přihlašování do aplikace OneDrive, zkontrolujte následující informace:

Vaše OneDrive verze musí být rovna nebo větší než verze 20.052.XXXX.XXXX. Pokud chcete zkontrolovat svou verzi, klikněte na modrou OneDrive v oznamovací oblast a vyberte Nápověda & Nastavení > Nastavení > **O aplikaci**.

Vaše síť může blokovat přenosy **g.live.com** **a oneclient.sfx.ms**. Pokud je tento přenos zablokovaný, OneDrive se aktualizovat. Pracujte se správcem sítě, abyste měli přístup k těm adresm URL. [Tyto koncové body by](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) měly být dosažitelné pro zákazníky, kteří používají Microsoft 365 plány.

Pokud potřebujete ručně získat aktuální verzi OneDrive, navštivte [https://aka.ms/getonedrive](https://aka.ms/getonedrive) stránku .
