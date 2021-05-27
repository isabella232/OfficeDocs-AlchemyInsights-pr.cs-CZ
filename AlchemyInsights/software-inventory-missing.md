---
title: Inventář softwaru chybí nebo je nepřesný
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676141"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>Inventář softwaru chybí nebo je nepřesný

Inventář softwaru v Threat and Vulnerability Management (TVM) je seznam známých softwaru ve vaší organizaci s oficiálními výčty společných platforem (CPE).

Softwarové produkty bez oficiální cpe nemají publikované chyby zabezpečení. Inventář obsahuje také podrobnosti, jako je jméno dodavatele, počet nedostatků, hrozby a počet exponovaných zařízení.

Změny softwaru na zařízeních se obvykle projeví na portálech zabezpečení do dvou hodin. Někdy to ale může trvat déle. Momentálně není žádný způsob, jak vynutit synchronizaci. jedná se o průběžné průběžné hodnocení.

Pokud jste provedli změnu softwaru a změna se přesně neprojeví v TVM po 5 hodinách, postupujte takto:

1. Informace o tom, jak byl software zjištěn, si můžete zjistit v části s důkazy softwaru.
1. Ujistěte se, že je software podporovaný. Software může být viditelný jenom na úrovni zařízení, i když ho v současné době Threat and Vulnerability Management. K dispozici jsou ale jenom omezená data.
1. Postup hlášení nepřesnosti z portálu najdete v článku [Nahlášení nepřesnosti](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).
   
    **Poznámka:** Hlášení nepřesnosti z portálu MDE je jednosměnný kanál k technice. Pokud je problém naléhavý, otevřete lístek podpory.

Další informace najdete v tématu [Inventář softwaru – Threat and Vulnerability Management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).