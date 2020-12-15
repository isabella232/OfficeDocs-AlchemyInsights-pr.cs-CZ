---
title: Nastavení ochrany osobních údajů v Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676974"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Nastavení ochrany osobních údajů v Microsoft Edge

Ve výchozím nastavení, pokud je Microsoft Edge nasazený na platformách nepoužívajících systém Windows, nejsou Microsoftu odesílána diagnostická data a informace o webu. Pokud je ale Microsoft Edge nasazený ve Windows 10, budou diagnostická data a informace o webu odesílány podle [nastavení Windows Diagnostic data](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).

Pokud chcete nakonfigurovat, jak Microsoft Edge zpracovává shromažďování dat pro vaši organizaci, použijte následující zásady skupiny:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Tato zásada umožňuje vykazování využití a dat souvisejících s chybou.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Tato zásada odešle informace o webu, které se používají ke zlepšení služeb Microsoftu.

Další informace najdete v článku [Konfigurace nastavení zásad](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).