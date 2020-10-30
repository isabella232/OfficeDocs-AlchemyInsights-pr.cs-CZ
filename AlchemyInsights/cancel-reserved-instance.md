---
title: Zrušení rezervace
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807363"
---
# <a name="cancelling-reservation"></a>Zrušení rezervace

- **Samoobslužné služby:** Rezervovanou instanci můžete zrušit nebo vyměnit pomocí [portálu Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vyberte rezervaci a klikněte na refundace nebo Exchange. Uvědomte si, že u objednávky rezervací musíte mít přístup vlastníka k Exchangi nebo vrácení peněz. Přístup pouze k rezervaci vám neumožní pokračovat v refundaci nebo Exchangi. Zeptejte se vlastníka objednávky rezervací, aby vám poskytl přístup vlastníka k objednávce rezervací.
- **Zásady Exchange:** Můžete si vyměnit rezervaci pro jinou rezervaci stejného typu – neexistují **žádné sankce** při výměně rezervací. Celkový závazek s novou výhradou by měl být větší než součet částky refundace vyměněné rezervace a budoucích měsíčních plateb (Pokud je to možné).
- **Zásady vracení peněz:** Součet refundace a zrušené budoucí platby nemohou překročit $50 000 USD v okně s dvanáctiměsíčním měsícem. V **současné době neplatíme žádné sankce** za vrácení peněz, které by mohly být účtovány budoucími náhradami.  
    **Výjimky:** Funkce samoobslužná výměna a zrušení nejsou pro zákazníky s podnikovou vládou USA k dispozici.
- Podpora **rozhraní API a PS/CLI** není dostupná pro zrušení a refundaci [automatických výměn a refundací pro Azure rezervací](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) .
- Funkce Samoobslužné výměny a rušení se nehodí pro zákazníky z dohod spojených s vládou USA. Podporují se i další typy předplatného pro vládní organizace včetně placeného placení a CSP.

Další informace: [zpracování transakcí vracení a výměny](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Další informace: [zásady výměny a refundace](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Další otázky: [navštivte vyhrazené instance](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) .

**Výměna existující rezervované instance (samoobslužné služby)**

Můžete si vyměnit rezervaci pro další rezervaci stejného typu. Můžete také vrátit rezervaci, až $50 000 USD za rok, pokud ji už nepotřebujete. Funkce Samoobslužné výměny a rušení se nehodí pro zákazníky z dohod spojených s vládou USA. Podporují se i další typy předplatného pro vládní organizace včetně placeného placení a CSP. Abyste mohli provést výměnu nebo refundaci existující rezervaci, musíte mít v pořadí rezervací oprávnění Vlastník.

Následující kroky se týkají postupu dokončení transakce

1. Přihlaste se ke svému [portálu Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vyberte rezervace, které chcete refundaci, a klikněte na **Exchange** .
2. Vyberte produkt VM, který chcete koupit, a zadejte množství. [Před nákupem](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy) se ujistěte, že je nový nákup větší než vrácená hodnota.
3. Kontrola a dokončení transakce

**Refundace rezervované instance**

Pokud chcete vrátit rezervaci, přejděte na **Detaily rezervací** a klikněte na **refundace** .

**Nominální refundace:**

**Příklad pro-dávku a minimální požadavek pro refundaci a Exchange**  
Příklad rezervace:

- Zakoupíte jednoletý termín RI pro $120 1. ledna
- 7. dubna, kterou chcete vrátit, nebo si vyměňovat tuto rezervaci
- Vzhledem k tomu, že rezervace je za 97 dnů živá, dostanete (1-97/365) * $120 zpátky. (například $88,1). V současné době není k dispozici žádná pokuta
- Při výměně by váš nový nákup měl být větší než $88,1
- V současné době neexistuje žádné snížení náhrad

**Příklad rezervace plánu fakturace:**

- Koupíte si jednoletý termín RI pro $10 za měsíc
- 7. dubna, kterou chcete vrátit, nebo si vyměňovat tuto rezervaci
- Od poslední platby uplynulo 7 dnů, získáte (1-7/31) * $10 zpátky. (například $7,74)
- Zrušení budoucích plateb je $80. V současné době není k dispozici žádná pokuta
- Toto zrušení odečte $87,74 od vás limit $50 000 refundace
- V případě výměny by měla být celková hodnota nového nákupu větší než $87,74

**Doporučené dokumenty**

- [Jak se zpracovávají transakce vracení a Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Zásady výměny a refundace](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)