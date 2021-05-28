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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696915"
---
# <a name="11-call-recording"></a>Nahrávání hovorů 1:1

Pokud je **tlačítko Spustit záznam** v hovoru 1:1 šedé, musíte změnit nastavení zásad pro ovlivněné uživatele.   

Od 31. května 2021 začneme vynucovat novou Teams hovory *AllowCloudRecordingForCalls*. Před touto změnou je záznam hovoru 1:1 řízený zásadou *AllowCloudRecording* Teams schůzek. Tato změna je zdokumentována v příspěvku Centra zpráv: [(aktualizováno) 1:1 Úvod](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)zásad nahrávání hovorů .  

*AllowCloudRecordingForCalls*   Možnost zásady volání je ve **$False** nastavená. Pokud chcete všem uživatelům blokovat nahrávání hovorů 1:1, nemusíte nic udělat.  

Pokud chcete povolit nahrávání hovorů pro všechny uživatele v hovoru 1:1, Teams PowerShellu spustit následující rutinu: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Můžete také vytvořit novou zásadu a nastavit **možnost -AllowCloudRecordingForCalls** tak, aby $true a přiřazovat je uživatelům.  

Další informace najdete v článku 1:1 Ovládací prvky zásad nahrávání hovorů [jsou (téměř!) Tady](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
