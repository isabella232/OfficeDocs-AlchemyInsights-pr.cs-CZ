---
title: Zrušení rezervace
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931226"
---
# <a name="cancelling-reservation"></a>Zrušení rezervace

- **Samoobslužné funkce:** Rezervované instance můžete sami zrušit nebo vyměnit přes [portál Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vyberte rezervaci a klikněte na refundaci nebo výměnu. Upozorňujeme, že pro výměnu nebo refundaci musíte mít přístup vlastníka k objednávce rezervace. Přístup jenom k rezervacím vám neumožní pokračovat v refundaci nebo výměně. Požádejte vlastníka objednávky rezervace, aby vám k ní dal přístup.
- **Zásady výměny:** Rezervaci můžete vyměnit za jinou rezervaci stejného typu – za výměnu rezervace **nebudete penalizováni**. Celkový závazek nové rezervace by měl být vyšší než součet refundované částky vyměněné rezervace a budoucích měsíčních plateb (v příslušných případech).
- **Zásady refundace:** Součet refundované částky a zrušených budoucích plateb nesmí ve 12 kalendářních měsících překročit 50 000 USD. **Momentálně refundace nepenalizujeme**, což se ale v budoucnu může změnit.  
    **Výjimky:** Samoobslužná výměna a zrušení nejsou dostupné zákazníkům smlouvy Enterprise ve státní správě USA.
- Podpora pro **API/PS/CLI** není dostupná pro zrušení a refundace. [Samoobslužné výměny a refundace za rezervace Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Samoobslužná výměna a zrušení nejsou dostupné zákazníkům smlouvy Enterprise ve státní správě USA. Podporované jsou jiné typy předplatného státní správy USA, včetně platby typu průběžná platba a CSP.

Další informace: [Jak se zpracovávají transakce vrácení a výměn](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Další informace: [Zásady výměny a refundace](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Další otázky: [Podívejte se na dokumenty o rezervovaných instancích](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Výměna existující rezervované instance (samoobslužná funkce)**

Rezervaci můžete vyměnit za jinou rezervaci stejného typu. Rezervaci můžete refundovat do výše 50 000 USD ročně, pokud už ji nepotřebujete. Samoobslužná výměna a zrušení nejsou dostupné zákazníkům smlouvy Enterprise ve státní správě USA. Podporované jsou jiné typy předplatného státní správy USA, včetně platby typu průběžná platba a CSP. Pro výměnu nebo refundaci existující rezervace musíte mít přístup vlastníka k objednávce rezervace.

Následující kroky vás provedou postupem pro dokončení transakce.

1. Přihlaste se k [portálu Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vyberte rezervace, které chcete refundovat, a klikněte na **Vyměnit**.
2. Vyberte produkt virtuálního počítače, který chcete koupit, a zadejte počet. Ujistěte se, že celková hodnota nákupu je vyšší než celková vrácená částka: [Určení správné velikosti virtuálního počítače před nákupem](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Kontrola a dokončení transakce

**Refundace za rezervovanou instanci**

Pokud chcete refundovat rezervaci, přejděte na **Podrobnosti rezervace** a klikněte na možnost **Refundace**.

**Poměrná refundace:**

**Poměry a příklady minimálních požadavků na refundaci a výměnu**  
Příklad počáteční rezervace:

- Prvního ledna si za 120 USD koupíte RI na rok.
- Sedmého dubna budete chtít tuto rezervaci refundovat nebo ji vyměnit.
- Vzhledem k tomu, že rezervace probíhala 97 dní, vrátí se vám (1–97/365) * 120 USD. (tj. 88,1 USD). Momentálně nemáte žádné penále za refundace.
- Při výměně by měl nový nákup mít hodnotu vyšší než 88,1 USD.
- Momentálně nemáte žádné penále za refundaci.

**Příklad rezervace fakturačního plánu:**

- Koupíte si RI na rok za 10 USD měsíčně.
- Sedmého dubna budete chtít tuto rezervaci refundovat nebo ji vyměnit.
- Od poslední platby uběhlo 7 dní, vrátí se vám (1–7/31) * 10 USD. (tj. 7,74 USD).
- Zrušené budoucí platby mají hodnotu 80 USD. Momentálně nemáte žádné penále za refundace.
- Zrušením se z vašeho limitu refundací o výši 50 000 USD odečte 87,74 USD.
- Při výměně by měl nový nákup mít hodnotu vyšší než 87,74 USD.

**Doporučené dokumenty**

- [Jak se zpracovávají transakce vrácení a výměn](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Zásady výměny a refundace](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)