---
title: Pozastavení naplánovaných aktualizací
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721548"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="c5e75-102">Pozastavení naplánovaných aktualizací</span><span class="sxs-lookup"><span data-stu-id="c5e75-102">Pausing scheduled updates</span></span>

<span data-ttu-id="c5e75-103">Pokud je příkaz Pause (pozastavit), zařízení nezpracovávají příkaz, dokud se nevrátí do Intune.</span><span class="sxs-lookup"><span data-stu-id="c5e75-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="c5e75-104">Zařízení proto může mít:</span><span class="sxs-lookup"><span data-stu-id="c5e75-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="c5e75-105">Nainstalovanou aktualizaci naplánovali před vrácením se změnami.</span><span class="sxs-lookup"><span data-stu-id="c5e75-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="c5e75-106">Vypnuté, když jste vypnuli příkaz pozastavit.</span><span class="sxs-lookup"><span data-stu-id="c5e75-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="c5e75-107">V tomto případě se může stát, že když zařízení byla zapnutá, můžou si před vrácením se se změnami stáhnout a nainstalovat naplánované aktualizace.</span><span class="sxs-lookup"><span data-stu-id="c5e75-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>