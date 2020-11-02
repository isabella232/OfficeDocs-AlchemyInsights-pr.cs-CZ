---
title: Fakturace pro nákup rezervované instance
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823029"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fakturace pro nákup rezervované instance

Rezervovaná instance je účtována způsobu platby, který je spojený s předplatným, které jste vybrali při nákupu. Typem předplatného musí být smlouva Enterprise (číslo nabídnutí: MS-AZR-0017P), plaťte podle sebe-Go (číslo nabídnutí: MS-AZR-0003P), smlouva zákazníka nebo CSP společnosti Microsoft.

- U předplatného podniku se poplatky odečtou od měnového zůstatku kreditu pro přihlášení nebo jako poplatky za převzetí.
- U předplatného s platbou po vás budou poplatky účtovány na platební kartu nebo na platební způsob platby.

**Zrušení rezervace**

- **Samoobslužné služby:** Rezervovanou instanci můžete zrušit nebo vyměnit pomocí [portálu Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vyberte rezervaci a klikněte na refundace nebo Exchange. Uvědomte si, že u objednávky rezervací musíte mít přístup vlastníka k Exchangi nebo vrácení peněz. Přístup pouze k rezervaci vám neumožní pokračovat v refundaci nebo Exchangi. Zeptejte se vlastníka objednávky rezervací, aby vám poskytl přístup vlastníka k objednávce rezervací.
- **Zásady Exchange:** Můžete si vyměnit rezervaci pro jinou rezervaci stejného typu – neexistují **žádné sankce** při výměně rezervací. Celkový závazek s novou výhradou by měl být větší než součet částky refundace vyměněné rezervace a budoucích měsíčních plateb (Pokud je to možné).
- **Zásady vracení peněz:** Součet refundace a zrušené budoucí platby nemohou překročit $50 000 USD v okně s dvanáctiměsíčním měsícem. V **současné době neplatíme žádné sankce** za vrácení peněz, které by mohly být účtovány budoucími náhradami.

**Výjimky:** Funkce samoobslužná výměna a zrušení nejsou pro zákazníky s podnikovou vládou USA k dispozici.

- Podpora **rozhraní API a PS/CLI** není dostupná pro zrušení a refundaci [automatických výměn a refundací pro Azure rezervací](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) .
- Funkce Samoobslužné výměny a rušení se nehodí pro zákazníky z dohod spojených s vládou USA. Podporují se i další typy předplatného pro vládní organizace včetně placeného placení a CSP.

Další informace: [jak se zpracovávají transakce vracení a Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Další informace: [zásady Exchange a refundace náhrad](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) další otázky: [navštivte vyhrazené instance](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) .

**Výměna existující rezervované instance (samoobslužné služby)**

Můžete si vyměnit rezervaci pro další rezervaci stejného typu. Můžete také vrátit rezervaci, až $50 000 USD za rok, pokud ji už nepotřebujete. Funkce Samoobslužné výměny a rušení se nehodí pro zákazníky z dohod spojených s vládou USA. Podporují se i další typy předplatného pro vládní organizace včetně placeného placení a CSP. Abyste mohli provést výměnu nebo refundaci existující rezervaci, musíte mít v pořadí rezervací oprávnění Vlastník.

Následující kroky se týkají postupu dokončení transakce

1. Přihlaste se k [portálu Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vyberte rezervace, které chcete refundaci, a klikněte na **Exchange** 2. Vyberte produkt VM, který chcete koupit, a zadejte množství. [Před nákupem](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)se ujistěte, že je nový nákup větší než vrácená hodnota.
3. Zkontrolujte a dokončete transakci.

**Refundace rezervované instance**

Pokud chcete vrátit rezervaci, přejděte na **Detaily rezervací** a klikněte na **refundace** .

**Nominální refundace:**

**Příklad pro-dávku a minimální požadavek pro refundaci a Exchange** Příklad rezervace:

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

**Nelze zobrazit fakturu za poslední fakturační období**

Existují některé možné důvody, proč nemůžete fakturu zobrazit:

- Máte měsíční kreditovou částku s předplatným, o kterou jste nepřekročili nebo máte bezplatnou zkušební verzi. Faktura se generuje jenom v případě, že dlužíte peníze.
- Je kratší než 30 dní od dne, kdy jste přihlášeni k Azure
- Faktura ještě není vygenerovaná. Počkat na konec fakturačního období
- Pokud nejste správce účtu, nemusí být starší faktury k dispozici

**Stažení faktury z Azure Portal (. PDF)**

- Výběr předplatného na stránce [předplatná](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) na portálu Azure jako [uživatel s přístupem k fakturám](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Výběr **faktur**
- Kliknutím na **stáhnout fakturu** zobrazíte kopii faktury ve formátu PDF. Pokud [nevidíte fakturu za poslední fakturační období?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice) **Not available**

**Příjem vaší faktury v e-mailu (. PDF)**

- Vyberte své předplatné ze stránky [předplatná](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Klikněte na **faktury** a odešlete e-mailem fakturu
- Klikněte na přijmout **v** a přijměte podmínky. U každého předplatného, které vlastníte, budete muset souhlasit.

Poznámka: Pokud nebudete po provedení těchto kroků dostávat e-maily, ujistěte se, že je vaše e-mailová adresa ve [svém profilu](https://account.windowsazure.com/profile) správná.

**Stažení dat o využití z portálu Azure**

- Přihlaste se do [centra účtů Azure](https://account.windowsazure.com/Subscriptions) jako [správce účtu](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) .
- Vyberte předplatné, pro které chcete informace o faktuře a používání
- Výběr **historie fakturace**
- Výběrem **Zobrazit aktuální výkaz** zobrazíte odhad nákladů v době vygenerování odhadu.
- Pokud chcete stáhnout denní data o využití jako soubor CSV, vyberte **Stáhnout využití** . Pokud se zobrazí dvě verze, Stáhněte si verzi 2

Další otázky: [navštivte vyhrazené instance](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) .

**Doporučené dokumenty**

- [Základy fakturace](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Principy používání rezervované instance slevy](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Stažení nebo zobrazení dat fakturace a denního používání faktur Azure](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Principy používání rezervované instance slevy](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Princip využití rezervované instance pro předplatné s platbou na váš tarif](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Principy vyhrazeného využití instance pro váš Podnikový zápis](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Poplatky za software Windows nezahrnuté v rezervovaných instancích](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervované instance programu partner Central Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)