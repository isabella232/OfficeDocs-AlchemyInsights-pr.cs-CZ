---
title: Vynucení limitu pro příjem poštovní schránky
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/31/2021
ms.locfileid: "59315835"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Vynucení limitu pro příjem poštovní schránky

Microsoft nedávno začal vynucovat mezní hodnotu 3600 zpráv za hodinu pro každou poštovní schránku. Další informace najdete v článku [Exchange Online limity](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). Microsoft 365 poštovní schránky, které do hodiny dostanou přes 3 600 zpráv, jsou na dalších 60 minut omezení. 

Kromě toho se použijí dvojice odesílatelů a příjemců (SRP), které blokují zprávy přijaté poštovní schránkou Microsoft 365 od určitého odesílatele. Pokud jeden odesílatel pošle určitému příjemci přes 33 % z celkové mezní hodnoty nebo 1200 zpráv za časovou hodinu, limit srpnové aktualizace se otevře a poštovní schránka už zprávy od tohoto odesílatele nepřijímá. Všimněte si, že:

- Tento limit je aplikace pro e-maily přijaté od jiných tenantů, místních nebo internetových odesílatelů.
- Doručování e-mailů do poštovní schránky je zablokované na dalších 60 minut. 
- Odesílatelům těchto poštovních schránek se zobrazí zpráva o nedoručení (5.2.121 nebo 5.2.122), která uvádí, že poštovní schránka překročila maximální prahovou hodnotu doručení. V rámci tenanta (pošta v rámci stejného tenanta) se dál doručuje.
- Při použití limitu SRP bude přijímající poštovní schránka dál přijímat zprávy od jiných odesílatelů.

Správci můžou sledovat aktuální aktivitu poštovní schránky tak, že přistupují k nové sestavě a můžou získat přehled v Centru pro správu Exchange s názvem "Poštovní schránky překračující limity příjmu". Přehled se zobrazí jenom v případě, že klient má urážející poštovní schránky, zatímco sestava se vždycky zobrazuje na řídicím panelu, ale je prázdná, pokud tenant nemá poštovní schránky, které se urážet.

Další informace o limitech pro přijímání přehledů najdete v článku Poštovní schránky překračující přehled o přijímajících limitech [v novém EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights).

Další informace o sestavě překročení limitů příjmu najdete v článku Poštovní schránky překračující limity příjmu v nové sestavě [EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report).