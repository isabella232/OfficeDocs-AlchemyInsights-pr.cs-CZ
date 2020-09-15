---
title: Výměna klasického kořenového webu s moderním webem
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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691172"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Výměna klasického kořenového webu s moderním webem

Pokud je vaše prostředí nastavené před duben 2019, můžete svůj kořenový web změnit na moderní web pomocí Microsoft PowerShellu:

- Pokud máte jiný web, který chcete použít jako kořenový web, můžete [tento kořenový web nahradit (zaměňovat)](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - Pomocí metody [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zaměníte umístění webu s jiným webem při archivaci původního webu. K dispozici pro týmový web (nepřipojený ke skupině) a komunikační Web. 

- Brzy budou zavedeny další možnosti, které vám umožní používat obsah na webu, ale převést existující web na komunikační Web. 
>[!Important]
>Tyto možnosti budou postupně shrnuty. Pokračujte v kontrole centra zpráv pro aktualizace. 

## <a name="known-issues-with-swapping-sites"></a>Známé problémy při záměně webů

- Cílový web může vrátit chybu "not found" (HTTP 404) po krátkou dobu.
- Abyste mohli aktualizovat index vyhledávání, bude potřeba obsah znovu projít. Není nutný žádný ruční krok – provede se to automaticky.
- Vše závislé na "statických" odkazech (například synchronizace souborů a soubory OneNotu) bude nutné ručně opravit.
- Pokud byl zdrojový web webem organizace – příspěvky, aktualizujte adresu URL.Získejte seznam všech organizačních webů.
- Weby Project serveru bude pravděpodobně nutné ověřit, abyste se ujistili, že jsou pořád správně přidružené.
