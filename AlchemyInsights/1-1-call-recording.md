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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733842"
---
# <a name="11-call-recording"></a>Nahrávání hovorů 1:1

Správci teď musí provést akci, aby uživatelé mohli nahrávat hovory 1:1.
 
Od 12. dubna 2021 začneme vynucovat novou možnost Zásad volání do Teams *AllowCloudRecordingForCalls*. 

V současné době jsou možnosti nahrávání hovorů 1:1 řízeny možností *AllowCloudRecording* v zásadách schůzek v Teams. Pokud mají vaši uživatelé povoleno zaznamenávat schůzky v Teams, 1:1 hovory 1:1.

Pokud chcete všem uživatelům blokovat nahrávání hovorů 1:1, není nutné nic dělat. *Možnost zásady volání AllowCloudRecordingForCalls* se $False ve výchozím nastavení.

Tato změna je zdokumentovaná v následujícím příspěvku Centra zpráv: [(aktualizováno) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Úvod k zásadám nahrávání hovorů Pokud chcete nastavit možnost zásad volání teams, musíte [použít Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

**Povolení nahrávání hovorů v 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**Zakázání nahrávání hovorů v hovorech 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

