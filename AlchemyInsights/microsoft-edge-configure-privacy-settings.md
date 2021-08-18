---
title: Microsoft Edge nastavení ochrany osobních údajů
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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114165"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge nastavení ochrany osobních údajů

Pokud je Microsoft Edge na platformách, které nejsou Windows, diagnostická data a informace o webu se ve výchozím nastavení microsoftu neposílat. Pokud je Microsoft Edge nasazení na Windows 10, diagnostická data a informace o webu se odesílat podle nastavení diagnostických dat uživatelů Windows [diagnostických dat.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Pokud chcete nakonfigurovat, Microsoft Edge zpracovává shromažďování dat pro vaši organizaci, použijte následující zásady skupiny:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Tato zásada umožňuje vykazovat využití a data související s chybou.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Tato zásada odesílá informace o webu, které se používají ke zlepšení služby Microsoft.

Další informace najdete v tématu [Konfigurace nastavení zásad](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).