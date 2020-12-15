---
title: Změna Microsoft Edge pomocí proměnných adresáře dat místo hardcoded cest
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677026"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Změna Microsoft Edge pomocí proměnných adresáře dat místo hardcoded cest

Pokud chcete například ve Windows ukládat data profilu pod místní data aplikace uživatele místo ve výchozím umístění, nastavte zásady **UserDataDir** na **$ {local_app_data} \Edge\Profile**. 

Další informace najdete v tématu [Vytvoření proměnných adresář uživatelských dat Microsoft Edge](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).