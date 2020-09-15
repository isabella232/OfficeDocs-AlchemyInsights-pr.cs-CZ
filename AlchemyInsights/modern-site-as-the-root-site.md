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
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666863"
---
# <a name="modern-site-as-root-site"></a>Moderní web jako kořenový web

Začali jsme vycházet s novou funkcí, která vám umožní [vyměnit kořenový web klasického webu pomocí moderního webu](https://docs.microsoft.com/sharepoint/modern-root-site). Pomocí metody [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zaměníte umístění webu s jiným webem při archivaci původního webu. K dispozici pro týmový web (nepřipojený ke skupině) a komunikační Web.

>[!Important]
> Neodstraňujte klasický kořenový web a vytvořte moderní komunikační Web. Microsoft toto nepodporuje. Když odstraníte kořenový web, budou všechny SharePointové weby ve vaší organizaci nedostupné všem uživatelům, dokud web neobnovíte nebo nevytvoříte nový web na stejné adrese URL. Tuto funkci sdělujeme prostřednictvím centra zpráv. Měli byste očekávat, že ve vašem klientovi brzy zapnete funkci.

## <a name="known-issues-with-swapping-sites"></a>Známé problémy při záměně webů
- Cílový web může vrátit chybu "not found" (HTTP 404) po krátkou dobu.
- Abyste mohli aktualizovat index vyhledávání, bude potřeba obsah znovu projít. Zde není žádný ruční krok, který bude proveden automaticky.
- Vše závislé na "statických" odkazech (například synchronizace souborů a soubory OneNotu) bude nutné ručně opravit.
- Weby Project serveru bude pravděpodobně nutné ověřit, abyste se ujistili, že jsou pořád správně přidružené. 
