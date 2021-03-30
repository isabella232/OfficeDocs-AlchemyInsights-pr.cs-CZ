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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402408"
---
# <a name="configure-endpoint-dlp"></a>Konfigurovat ochranu před únikem informací pro koncové body

Ochrana před únikem informací koncového bodu Microsoft umožňuje rozšířit možnosti ochrany před únikem informací a sledování citlivých informací na zařízeních s Windows 10. Jakmile zařízení nahlásíte do správy zařízení, můžete vytvořit zásady ochrany před únikem informací, které budou vynucovat ochranná opatření pro položky. Pomocí Průzkumníka aktivit můžete sledovat aktivitu citlivých položek. Další informace najdete v článku [Onboarding zařízení do správy zařízení](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Jak začít používat ochranu před únikem informací koncového bodu:

- Ujistěte se, že máte odpovídající licence skladové jednotky (SKU) nebo předplatného. Další informace najdete v článku [Licence SKU nebo předplatného](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Zkontrolujte oprávnění potřebná k povolení správy zařízení, přístupu na stránku pro onboarding nebo zapnutí/vypnutí monitorování zařízení. Další informace najdete v článku na téma [Oprávnění](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Zařízení můžete zapojit do Správy zařízení, když budete postupovat podle návodu na onboarding nového zařízení. Pokud v části Dodržování předpisů M365 **Nastavení** chybí možnost Onboarding zařízení (náhled), zkontrolujte, jestli máte odpovídající licenci a oprávnění, na které se odkazuje výše. Další informace najdete v článku [Onboarding zařízení](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Vytvořte zásady ochrany před únikem informací, které ochrání vaše citlivé položky. Informace najdete v článku [Scénáře zásad ochrany před únikem informací koncových bodů](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Další informace o ochraně před únikem informací pro koncové body Microsoftu najdete v článku [Ochrana před únikem informací koncových bodů Microsoftu 365 (náhled)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Postup při Shromažďování důležitých dat, pokud je potřeba podpora:**

1. Stáhněte si MDATP Client Analyzer ve verzi Preview z [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. V okně cmd spusťte nástroj jako správce:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Po zobrazení výzvy „Zadejte počet minut potřebných ke shromáždění dat sledování:“, zadejte počet minut, které jsou potřeba k provedení scénáře.
5. Spustit scénář

Získaný výstup souboru ZIP se předá agentovi podpory.
