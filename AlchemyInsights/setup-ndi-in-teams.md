---
title: Zapnutí technologie NDI
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023515"
---
# <a name="turn-on-ndi-technology"></a>Zapnutí technologie NDI

Technologie NDI vyžaduje, aby se uživateli zapnuly dva kroky:

1. Správce tenanta musí povolit vlastnost AllowNDIStreaming v CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Po naplnění této změny musí koncový uživatel zapnout technologii NDI® pro svého konkrétního klienta z **Nastavení > oprávnění.**

Další informace najdete v tématu [Použití technologie NDI v Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
