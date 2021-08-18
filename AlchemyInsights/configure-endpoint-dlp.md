---
title: Konfigurovat ochranu před únikem informací pro koncové body
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323911"
---
# <a name="configure-endpoint-dlp"></a>Konfigurovat ochranu před únikem informací pro koncové body

Ochrana před únikem informací koncového bodu Microsoft umožňuje rozšířit možnosti ochrany před únikem informací a sledování citlivých informací na zařízeních s Windows 10. Jakmile zařízení nahlásíte do správy zařízení, můžete vytvořit zásady ochrany před únikem informací, které budou vynucovat ochranná opatření pro položky. Pomocí Průzkumníka aktivit můžete sledovat aktivitu citlivých položek. Další informace najdete v článku [Onboarding zařízení do správy zařízení](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Jak začít používat ochranu před únikem informací koncového bodu:

- Ujistěte se, že máte odpovídající licence skladové jednotky (SKU) nebo předplatného. Další informace najdete v článku [Licence SKU nebo předplatného](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Zkontrolujte oprávnění potřebná k povolení správy zařízení, přístupu na stránku pro onboarding nebo zapnutí/vypnutí monitorování zařízení. Další informace najdete v článku na téma [Oprávnění](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Zařízení můžete zapojit do Správy zařízení, když budete postupovat podle návodu na onboarding nového zařízení. Další informace najdete v článku [Onboarding zařízení](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Vytvořte zásady ochrany před únikem informací, které ochrání vaše citlivé položky. Informace najdete v článku [Scénáře zásad ochrany před únikem informací koncových bodů](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Další informace o ochraně před únikem informací pro koncové body Microsoftu najdete v článku [Ochrana před únikem informací koncových bodů Microsoftu 365 (náhled)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Postup při Shromažďování důležitých dat, pokud je potřeba podpora:**

1. Stáhněte [si MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).
1. V okně cmd spusťte nástroj jako správce:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Po zobrazení výzvy zadejte počet minut ke shromažďování **trasování:**, zadejte počet minut nutný ke spuštění scénáře.
1. Spusťte scénář.

Shromažďte výstup souboru ZIP, který chcete dát agentovi podpory.
