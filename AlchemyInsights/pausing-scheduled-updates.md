---
title: Pozastavení plánovaných aktualizací
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/30/2020
ms.locfileid: "46554912"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="346b7-102">Pozastavení plánovaných aktualizací</span><span class="sxs-lookup"><span data-stu-id="346b7-102">Pausing scheduled updates</span></span>

<span data-ttu-id="346b7-103">Když je vydán příkaz pauza, zařízení příkaz nezpracují až při příštím vrácení se změnami do Intune.</span><span class="sxs-lookup"><span data-stu-id="346b7-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="346b7-104">Z tohoto důvodu mohou mít vaše zařízení:</span><span class="sxs-lookup"><span data-stu-id="346b7-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="346b7-105">Před vrácením se změnami byly nainstalovány naplánované aktualizace.</span><span class="sxs-lookup"><span data-stu-id="346b7-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="346b7-106">Byl vypnut, když jste vydal příkaz pauza.</span><span class="sxs-lookup"><span data-stu-id="346b7-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="346b7-107">V takovém případě, když byla zařízení zapnutá, mohla stáhnout a nainstalovat naplánované aktualizace před vrácením se změnami.</span><span class="sxs-lookup"><span data-stu-id="346b7-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>