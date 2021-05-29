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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702083"
---
# <a name="11-call-recording"></a>Nahrávání hovorů 1:1

Pokud je **tlačítko Spustit záznam** v hovoru 1:1 šedé, musíte změnit nastavení zásad pro ovlivněné uživatele. Pokud chcete zkontrolovat nastavení zásad, spusťte diagnostiku pro ovlivněné uživatele tak, že napíšete **Diag: Teams 1:1 Nahrávání hovorů** výše.     

Od 31. května 2021 začneme vynucovat novou Teams hovory *AllowCloudRecordingForCalls*. Před touto změnou je záznam hovoru 1:1 řízený zásadou *AllowCloudRecording* Teams schůzek. Tato změna je zdokumentována v příspěvku Centra zpráv: [(aktualizováno) 1:1 Úvod](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)zásad nahrávání hovorů .  

*AllowCloudRecordingForCalls*   Možnost zásady volání je ve **$False** nastavená. Pokud chcete všem uživatelům blokovat nahrávání hovorů 1:1, nemusíte nic udělat.  

Pokud chcete povolit nahrávání hovorů pro všechny uživatele v hovoru 1:1, [Teams PowerShell](/microsoftteams/teams-powershell-install) spustit následující rutinu: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Můžete také vytvořit novou zásadu a nastavit **možnost -AllowCloudRecordingForCalls** tak, aby $true a přiřazovat je uživatelům.  

Další informace najdete v článku 1:1 Ovládací prvky zásad nahrávání hovorů [jsou (téměř!) Tady](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
