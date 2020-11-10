---
title: Chyba přihlášení na OneDrive AADSTS50011
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
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982431"
---
# <a name="onedrive-login-error-aadsts50011"></a>Chyba přihlášení na OneDrive AADSTS50011

Pokud se zobrazí chybová zpráva "AADSTS50011: adresa URL odpovědi zadaná v žádosti neodpovídá odpovědi" při přihlášení do aplikace OneDrive, zkontrolujte následující skutečnosti:

Vaše verze OneDrivu musí být stejná nebo větší než verze 20.052. XXXX. XXXX. Pokud chcete zkontrolovat svoji verzi, klikněte na modré ikoně OneDrivu v oznamovací oblasti a vyberte **& nastavení > nastavení >**.

Síť může blokovat provoz na **g.Live.com** a **oneclient.SFX.MS**. Pokud je tento přenos blokován, nemůže se OneDrive sám aktualizovat. Spolupracujte s vaším správcem sítě, abyste měli přístup k těmto adresám URL. [Tyto koncové body](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) by měly být dosažitelné pro zákazníky používající plány Microsoft 365.

Pokud potřebujete ručně získat aktuální verzi OneDrivu, navštivte [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
