---
title: V Centru zabezpečení nebyla nalezena žádná zpráva o předplatných.
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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544101"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>V Centru zabezpečení nebyla nalezena žádná zpráva o předplatných.

Pokud se při Centrum zabezpečení v programu Microsoft Defender zobrazí zpráva o tom, že se nenašla žádná předplatná, znamená to, že Azure Active Directory (AAD), který se používá k přihlášení uživatele k portálu, nemá Microsoft Defender ATP licenci.  

Licence Windows E5 a Office E5 jsou samostatné licence.

Otevřete případ podpory, pokud byla licence zakoupena, ale nebyla zřízena pro tuto instanci služby AAD. Buď máte: <br/>
-   Možný problém se zřizováním licencí.<br/>
-   Neúmyslně jste zřásekli licenci na jinou službu Microsoft AAD, než která se používá k ověřování ve službě.