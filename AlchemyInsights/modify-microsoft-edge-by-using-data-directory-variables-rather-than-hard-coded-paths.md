---
title: Úprava Microsoft Edge pomocí proměnných datového adresáře místo pevných cest
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035014"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Úprava Microsoft Edge pomocí proměnných datového adresáře místo pevných cest

Pokud chcete například ve Windows ukládat data profilu pod daty místní aplikace uživatele a ne do výchozího umístění, nastavte zásadu *UserDataDir* na **${local_app_data}\Edge\Profile**.

Další informace najdete v tématu [Vytvoření proměnných adresáře uživatelských dat](https://docs.microsoft.com/deployedge/microsoft-edge-policies)v Microsoft Edge .