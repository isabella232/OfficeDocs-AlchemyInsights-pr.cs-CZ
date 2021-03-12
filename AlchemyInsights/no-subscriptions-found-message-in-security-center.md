---
title: Zpráva o tom, že v Centru zabezpečení nebyla nalezena žádná předplatná
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713412"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Zpráva o tom, že v Centru zabezpečení nebyla nalezena žádná předplatná

Pokud se při přístupu k Centru zabezpečení v programu Microsoft Defender zobrazí zpráva "Nenašla se žádná předplatná", znamená to, že služba Azure Active Directory (AAD) použitá k přihlášení uživatele k portálu nemá licenci Microsoft Defenderu atp.  

Licence na Windows E5 a Office E5 jsou samostatné licence.

Otevřete případ podpory, pokud byla licence zakoupena, ale nebyla zřízena pro tuto instanci služby AAD. Máte buď: <br/>
-   Možný problém s zřizováním licencí.<br/>
-   Neúmyslně jste zřizaci licence jinému účtu Microsoft AAD, než se používá k ověřování ve službě.