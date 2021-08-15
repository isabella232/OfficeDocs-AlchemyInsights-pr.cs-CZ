---
title: Diagnostika problémů s přístupem k různým portům
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030895"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostika problémů s přístupem k různým portům

Pokud chcete vyřešit různé problémy s přístupem k portu, postupujte takto:

1. Zastavte nebo nastavte přidělení virtuálního počítače z portálu, restartujte virtuální počítač a otestujte ho znovu. 
2. Zkontrolujte nastavení sítě vašeho virtuálního počítače a zjistěte, jestli máte blokující přenos skupin zabezpečení sítě( NSG). Pomocí nástroje ověření toku [IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) adres můžete taky zkontrolovat, jestli sítě blokují přenosy, User-Defined Trasy (UDR) přesměrovává provoz zpátky do místního (výchozí trasa 0.0.0.0/0) nebo do síťového zařízení.
Pokud se po provedení výše uvedených kroků pořád vyskytnou problémy, zadejte název virtuálního počítače a port TCP, na který se pokoušíte poslat poštu, aby bylo možno dál diagnostikovat.

**Doporučené dokumenty**

[Omezení a doporučení pro posílání odchozích e-mailů přes port 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)