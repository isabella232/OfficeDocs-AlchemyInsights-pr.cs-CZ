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
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a><span data-ttu-id="1d5ed-102">Úprava Microsoft Edge pomocí proměnných datového adresáře místo pevných cest</span><span class="sxs-lookup"><span data-stu-id="1d5ed-102">Modify Microsoft Edge by using data directory variables rather than hard-coded paths</span></span>

<span data-ttu-id="1d5ed-103">Pokud chcete například ve Windows ukládat data profilu pod daty místní aplikace uživatele a ne do výchozího umístění, nastavte zásadu *UserDataDir* na **${local_app_data}\Edge\Profile**.</span><span class="sxs-lookup"><span data-stu-id="1d5ed-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the *UserDataDir* policy to **${local_app_data}\Edge\Profile**.</span></span>

<span data-ttu-id="1d5ed-104">Další informace najdete v tématu [Vytvoření proměnných adresáře uživatelských dat](https://docs.microsoft.com/deployedge/microsoft-edge-policies)v Microsoft Edge .</span><span class="sxs-lookup"><span data-stu-id="1d5ed-104">For more information, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/microsoft-edge-policies).</span></span>