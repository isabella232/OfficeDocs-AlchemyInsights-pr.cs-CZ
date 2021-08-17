---
title: Chyba 10061 rozhraní Winsock 1554
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083223"
---
# <a name="winsock-error-10061"></a>Chyba Rozhraní Winsock 10061

Tento kód chyby znamená, že Microsoft nemohl vytvořit soket TCP (připojení) s cílovým hostitelem. Nejpravděpodobnější příčinou této chyby je problém s konfigurací brány firewall. Pokud chcete problém vyřešit, zkontrolujte tato nastavení:

- Ověření konfigurace brány firewall pomocí informací v Microsoft 365 adres URL a [rozsahech IP adres](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Pokud je chyba specifická pro Exchange Online Protection (EOP), měli byste být dříve upozorněni na změnu Exchange Online Protection [IP adres.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Ověřte, že poskytovatel internetových služeb neblokuje port.

- Ověřte nastavení inteligentního hostitele a cílového serveru v konektorech.

Všimněte Microsoft 365, že příchozí  připojení tímto způsobem neblokuje.
