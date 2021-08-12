---
title: Výměna klasického kořenového webu pomocí moderního webu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 7209595f5cda9b31e53241d9d5696fa584ff5e5ab3d237aae28542bf7aec9398
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940812"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Výměna klasického kořenového webu pomocí moderního webu

Pokud jste prostředí nastavili před dubnem 2019, můžete svůj kořenový web změnit na moderní web pomocí Microsoft PowerShellu:

- Pokud máte jiný web, který chcete použít jako kořenový web, můžete ho nahradit [(zaměnit).](https://docs.microsoft.com/sharepoint/modern-root-site) 
    - Funkce [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) slouží k výměně umístění webu s jiným webem při archivaci původního webu. K dispozici pro týmový web (není připojený ke skupině) i pro komunikační web. 

- Brzy budou zavedeny další funkce, které vám umožní dál používat obsah na webu, ale stávající web převést na komunikační web. 
>[!Important]
>Tyto funkce se budou postupně rozšiřovat. Pokračujte v kontrole aktualizací v Centru zpráv. 

## <a name="known-issues-with-swapping-sites"></a>Známé problémy s vyměňování webů

- Cílový web může krátkou dobu vrátit chybu "nenal." (HTTP 404).
- Aby se index hledání aktualizovat, bude potřeba obsah znovu prohledat. Není nutný žádný ruční krok – tento krok se provádí automaticky.
- Všechno, co závisí na "statických" odkazech (například Synchronizace souborů a OneNote souborů), bude muset být ručně opraveno.
- Pokud byl zdrojový web zpravodajský web organizace, aktualizujte adresu URL. Získejte seznam všech zpravodajských webů organizace.
- Project Serverové weby je možná potřeba ověřit, aby se zajistilo, že jsou pořád správně spojené.
