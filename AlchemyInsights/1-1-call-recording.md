---
title: Nahrávání hovorů 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314377"
---
# <a name="11-call-recording"></a>Nahrávání hovorů 1:1

Pokud je **tlačítko Spustit záznam** v hovoru 1:1 šedé, musíte změnit nastavení zásad pro ovlivněné uživatele. Pokud chcete zkontrolovat nastavení zásad, spusťte diagnostiku pro ovlivněné uživatele tak, že napíšete **Diag: Teams 1:1 Nahrávání hovorů** výše.     

Od 31. května 2021 začneme vynucovat novou Teams hovory *AllowCloudRecordingForCalls*. Před touto změnou je záznam hovoru 1:1 řízený zásadou *AllowCloudRecording* Teams schůzek. Tato změna je zdokumentována v příspěvku Centra zpráv: [(aktualizováno) 1:1 Úvod](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)zásad nahrávání hovorů .  

*AllowCloudRecordingForCalls*   Možnost zásad volání je ve **$False** nastavená. Pokud chcete všem uživatelům blokovat nahrávání hovorů 1:1, nemusíte nic udělat.  

Pokud chcete povolit nahrávání hovorů pro všechny uživatele v hovoru 1:1, [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) spustit následující rutinu: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Můžete také vytvořit novou zásadu a nastavit **možnost -AllowCloudRecordingForCalls** tak, aby $true a přiřadit je uživatelům.  

Další informace najdete v článku 1:1 Ovládací prvky zásad nahrávání hovorů [jsou (téměř!) Tady](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
