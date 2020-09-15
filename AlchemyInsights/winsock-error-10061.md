---
title: 1554 chyba Winsock 10061
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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698855"
---
# <a name="winsock-error-10061"></a>Chyba rozhraní Winsock 10061

Tento chybový kód znamená, že Microsoft nemůže vytvořit soket TCP (připojení) s cílovým hostitelem. Nejpravděpodobnější příčinou této chyby je problém s konfigurací brány firewall. Tento problém můžete vyřešit kontrolou těchto nastavení:

- Ověření konfigurace brány firewall informacemi v [adresách URL a IP adres Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Pokud je chyba specifická pro Exchange Online Protection (EOP), měli byste se dřív upozornit na změnu [IP adres ochrany Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Ověřte, že port neblokoval váš poskytovatel internetových služeb.

- Ověřte nastavení inteligentního hostitele a cílového serveru ve svých konektorech.

Upozorňujeme, že Microsoft 365 tímto způsobem neblokuje *příchozí* připojení.
