---
title: Výchozí Outlook popisku se nepou ít
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454565"
---
# <a name="default-outlook-label-setting-not-applied"></a>Výchozí Outlook popisku se nepou ít

Pokud se výchozí nastavení štítků Outlook nevyužívá správně a použije se jiný popisek nebo žádný popisek, může docházet k známém problému (MC277818) a měli byste udělat jednu z těchto 2 možností, jak tento problém vyřešit:

**Možnost 1:**

1. Přejděte na Microsoft 365 Compliance Center > **Solutions**  >  **Information Protection**.
1. Vyberte **Zásady štítků** a vyberte zásadu popisků, kterou potřebujete upravit ( u zásady popisků není správně nastavené nastavení **OutlookDefaultlabel.** Pokud chcete toto nastavení zobrazit, spusťte **Get-labelpolicy** a pak vyberte **Upravit zásadu**.
1. Vyberte **Další,** dokud se v dialogovém okně Nastavení zásad neuvidí  nastavení Použít tento výchozí popisek pro  e-maily **,** které je dostupné, pokud v dialogovém okně Nastavení zásad vyberete Požadovat, aby uživatelé u dědiků a dokumentů nálepce.
1. V dialogovém **okně Apply a default label to documents** (Použít výchozí popisek u dokumentů) v rozevíracím seznamu vyberte None **(Žádné).**
1. Pokud **chcete uložit** nastavení štítků, vyberte Další a Odeslat. 

**Možnost 2:**

V Centru zabezpečení a [dodržování předpisů Powershellu](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)můžete pomocí Set-LabelPolicy změnit popisek **OutlookDefaultlabel** na **None** v {OutlookDefaultLabel="None"}.

Spustit: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Další informace o výchozích popiscích Outlook najdete v tématu Nastavení [jiného výchozího](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)popisku Outlook .