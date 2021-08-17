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
ms.openlocfilehash: 29383643e6867bca7fd31774a9594b82fdc080bb0e7254141e8c883ad861075e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886132"
---
# <a name="11-call-recording"></a>Nahrávání hovorů 1:1

Pokud je **tlačítko Spustit záznam** v hovoru 1:1 šedé, musíte změnit nastavení zásad pro ovlivněné uživatele. Pokud chcete zkontrolovat nastavení zásad, spusťte diagnostiku pro ovlivněné uživatele tak, že napíšete **Diag: Teams 1:1 Nahrávání hovorů** výše.     

Od 31. května 2021 začneme vynucovat novou Teams zásady volání *AllowCloudRecordingForCalls*. Před touto změnou je záznam hovoru 1:1 řízený Teams schůzek.  Tato změna je zdokumentována v příspěvku Centra zpráv: [(aktualizováno) 1:1 Úvod](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)zásady nahrávání hovorů .  

*AllowCloudRecordingForCalls*   Možnost zásady volání je ve **$False** nastavená. Pokud chcete všem uživatelům blokovat nahrávání hovorů 1:1, nemusíte nic udělat.  

Pokud chcete povolit nahrávání hovorů pro všechny uživatele v hovoru 1:1, [Teams PowerShellu](https://docs.microsoft.com/microsoftteams/teams-powershell-install) spustit následující rutinu: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Můžete také vytvořit novou zásadu a nastavit **možnost -AllowCloudRecordingForCalls** tak, aby $true a přiřazovat je uživatelům.  

Další informace najdete v článku 1:1 Ovládací prvky zásad nahrávání hovorů [jsou (téměř!) Tady](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
