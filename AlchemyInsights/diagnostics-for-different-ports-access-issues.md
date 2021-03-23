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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035003"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="97f39-102">Diagnostika problémů s přístupem k různým portům</span><span class="sxs-lookup"><span data-stu-id="97f39-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="97f39-103">Pokud chcete vyřešit různé problémy s přístupem k portu, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="97f39-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="97f39-104">Zastavte nebo nastavte přidělení virtuálního počítače z portálu, restartujte virtuální počítač a otestujte ho znovu.</span><span class="sxs-lookup"><span data-stu-id="97f39-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="97f39-105">Zkontrolujte nastavení sítě vašeho virtuálního počítače a zjistěte, jestli máte blokující přenos skupin zabezpečení sítě( NSG).</span><span class="sxs-lookup"><span data-stu-id="97f39-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="97f39-106">Pomocí nástroje ověření toku [IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) adres můžete taky zkontrolovat, jestli sítě blokují přenosy, User-Defined Trasy (UDR) přesměrovává provoz zpátky do místního (výchozí trasa 0.0.0.0/0) nebo do síťového zařízení.</span><span class="sxs-lookup"><span data-stu-id="97f39-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="97f39-107">Pokud se po provedení výše uvedených kroků pořád vyskytnou problémy, zadejte název virtuálního počítače a port TCP, na který se pokoušíte poslat poštu, aby bylo možno dál diagnostikovat.</span><span class="sxs-lookup"><span data-stu-id="97f39-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="97f39-108">**Doporučené dokumenty**</span><span class="sxs-lookup"><span data-stu-id="97f39-108">**Recommended Documents**</span></span>

[<span data-ttu-id="97f39-109">Omezení a doporučení pro posílání odchozích e-mailů přes port 25</span><span class="sxs-lookup"><span data-stu-id="97f39-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)