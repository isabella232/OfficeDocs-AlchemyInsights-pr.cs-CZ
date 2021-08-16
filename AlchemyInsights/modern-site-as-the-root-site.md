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
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000379"
---
# <a name="modern-site-as-root-site"></a>Moderní web jako kořenový web

Začali jsme zaměňovat novou funkci, která vám umožní vyměnit váš klasický kořenový web za [moderní web.](https://docs.microsoft.com/sharepoint/modern-root-site) Funkce [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) slouží k výměně umístění webu s jiným webem při archivaci původního webu. K dispozici pro týmový web (není připojený ke skupině) i pro komunikační web.

>[!Important]
> Pokud chcete vytvořit moderní komunikační web, neodstraňovat klasický kořenový web. Microsoft to nepodporuje. Odstraněním kořenového webu nebudou SharePoint všechny weby ve vaší organizaci přístupné všem uživatelům, dokud web obnovíte nebo nevytváříte nový web na stejné adrese URL. Tuto funkci budeme komunikovat prostřednictvím Centra zpráv. Měli byste očekávat, že funkce bude v tenantovi brzy zapnutá.

## <a name="known-issues-with-swapping-sites"></a>Známé problémy s vyměňování webů
- Cílový web může krátkou dobu vrátit chybu "nenal." (HTTP 404).
- Aby se index hledání aktualizovat, bude potřeba obsah znovu prohledat. Tady není nutný žádný ruční krok, tento krok se provádí automaticky.
- Všechno, co závisí na "statických" odkazech (například Synchronizace souborů a OneNote souborů), bude muset být ručně opraveno.
- Project Serverové weby je možná potřeba ověřit, aby se zajistilo, že jsou pořád správně spojené. 
