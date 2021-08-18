---
title: Moderní web jako kořenový web
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327595"
---
# <a name="modern-site-as-root-site"></a>Moderní web jako kořenový web

Začali jsme zaměňovat novou funkci, která vám umožní vyměnit váš klasický kořenový web za [moderní web.](https://docs.microsoft.com/sharepoint/modern-root-site) Funkce [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) slouží k výměně umístění webu s jiným webem při archivaci původního webu. K dispozici pro týmový web (není připojený ke skupině) i pro komunikační web.

**Důležité:** Pokud chcete vytvořit moderní komunikační web, neodstraňovat klasický kořenový web. Microsoft to nepodporuje. Odstraněním kořenového webu nebudou SharePoint všechny weby ve vaší organizaci přístupné všem uživatelům, dokud web obnovíte nebo nevytváříte nový web na stejné adrese URL. Tuto funkci budeme komunikovat prostřednictvím Centra zpráv. Měli byste očekávat, že funkce bude v tenantovi brzy zapnutá.

## <a name="known-issues-with-swapping-sites"></a>Známé problémy s vyměňování webů
- Cílový web může krátkou dobu vrátit chybu "nenal." (HTTP 404).
- Aby se index hledání aktualizovat, bude potřeba obsah znovu prohledat. Tady není nutný žádný ruční krok, tento krok se provádí automaticky.
- Všechno, co závisí na "statických" odkazech (například synchronizace souborů a OneNote souborů), bude muset být ručně opraveno.
- Project Serverové weby je možná potřeba ověřit, aby se zajistilo, že jsou pořád správně spojené. 
