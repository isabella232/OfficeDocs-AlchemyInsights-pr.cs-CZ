---
title: Fakturace za nákup rezervované instance
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820315"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fakturace za nákup rezervované instance

Nákup rezervované instance se účtuje podle způsobu platby vázaného na předplatné, které vyberete v okamžiku nákupu. Typ předplatného musí být smlouva enterprise (číslo nabídky: MS-AZR-0017P), Pay-As-You-Go (číslo nabídky: MS-AZR-0003P), Smlouva se zákazníky společnosti Microsoft nebo csp.

- U podnikového předplatného se poplatky odečtou z zůstatku peněžního závazku registrace nebo se účtují jako nadváže.
- U předplatného Pay-As-You-Go se poplatky účtují na platební kartu nebo způsob platby fakturou v rámci předplatného.

**Zrušení rezervace**

- **Samoobslužná služba:** Rezervovaný výskyt můžete zrušit nebo si vyměnit sami pomocí [portálu Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vyberte rezervaci a klikněte na refundaci nebo výměnu. Upozorňujeme, že k výměně nebo refundaci musíte mít přístup vlastníka k objednávce rezervace. Přístup jenom k rezervaci vám neumů e pokračovat v refundaci nebo výměně. Požádejte vlastníka objednávky rezervace, aby vám dal přístup k objednávce rezervace.
- **Zásady Exchange:** Rezervaci si můžete vyměnit za jinou rezervaci stejného typu – při výměně rezervací nejsou **žádné** postihy. Celkový závazek s novou rezervací by měl být větší než součet částky refundace vyměněné rezervace a budoucích měsíčních plateb (pokud je to možné)
- **Zásady refundace:** Součet refundace a zrušených budoucích plateb nesmí překročit 50 000 USD v 12měsíčním průběžném okně. V současné **době neúčtujeme žádnou penále** za refundace, ale můžeme ji účtovat z budoucích refundace.

**Výjimky:** Možnost samoobslužné výměny a zrušení není dostupná pro zákazníky se smlouvou US Government Enterprise Agreement

- **Podpora API / PS / CLI** není dostupná pro zrušení a refundace samoobslužných výměn a refundace za rezervace [Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Možnost samoobslužné výměny a zrušení není dostupná pro zákazníky se smlouvou US Government Enterprise Agreement. Podporují se další typy předplatného americké vlády, včetně služeb Pay-As-You-Go a CSP.

Další informace : [Zpracování transakcí vrácení](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) a výměny Další informace : Zásady [exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) a refundace Další otázky: Navštivte dokumenty [rezervované instance](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange stávající rezervované instance (samoobslužná služba)**

Rezervaci si můžete vyměnit za jinou rezervaci stejného typu. Pokud už rezervaci nepotřebujete, můžete refundovat rezervaci až do výše 50 000 USD ročně. Možnost samoobslužné výměny a zrušení není dostupná pro zákazníky se smlouvou US Government Enterprise Agreement. Podporují se další typy předplatného americké vlády, včetně placených služeb a csp. K výměně nebo refundaci stávající rezervace musíte mít přístup vlastníka k objednávce rezervace.

Následující kroky vám posouou pokyny k provedení transakce.

1.Přihlaste se k [portálu Azure Portal.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Vyberte rezervace, které chcete vrátit, a klikněte na **Exchange** 2. Vyberte produkt virtuálního počítače, který chcete koupit, a zadejte množství. Ujistěte se, že nový nákupní součet je víc než celkový výnos. Před nákupem určete [správnou velikost.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Zkontrolujte a dokončete transakci.

**Refundace za rezervovanou instanci**

Pokud chcete refundovat rezervaci, přejděte na **Podrobnosti rezervace** a klikněte na **Refundovat.**

**Pro-rated refundace:**

**Příklady provizí a minimálních požadavků pro refundaci a výměnu** Příklad rezervace předem:

- 1. ledna si zakoupíte roční období RI za 120 USD.
- 7. dubna chcete tuto rezervaci vrátit nebo vyměnit.
- Vzhledem k tomu, že rezervace je živě 97 dní, dostanete (1.97.365) * 120 Kč zpět. (tj. 88,1 Kč). V současné době neexistuje žádná penále za refundace.
- Při výměně by váš nový nákup měl být vyšší než 88,1 USD.
- V současné době neexistuje žádná penále za refundace.

**Příklad rezervace fakturačního plánu:**

- Zakoupíte si roční období RI za 10 USD měsíčně.
- 7. dubna chcete tuto rezervaci vrátit nebo vyměnit.
- Od poslední splátky za 7 dní dostanete (1.7.31) * 10 Kč zpět. (tj. 7,74 Kč)
- Zrušené budoucí platby jsou 80 Usd. V současné době neexistuje žádná penále za refundace.
- Toto zrušení vám odečte 87,74 USD od limitu refundace ve výši 50 000 Kč.
- Při výměně by celková hodnota nového nákupu měla být vyšší než 87,74 Kč.

**Fakturu za poslední fakturační období se nepodařilo zobrazit.**

Některé možné důvody, proč se vám faktura nemusí zobrazit:

- U předplatného máte měsíční kredit, který jste nepřekročili nebo máte bezplatnou zkušební verzi. Faktura se vygeneruje jenom v případě, že jste dlužní peníze.
- Je to méně než 30 dní ode dne, kdy jste se přihlásili k odběru Azure.
- Faktura se ještě nevygeneruje. Počkejte až do konce fakturačního období.
- Pokud nejste správcem účtu, starší faktury nemusí být pro vás dostupné.

**Stáhněte si fakturu z webu Azure Portal (.pdf)**

- Vyberte předplatné na stránce [Předplatná](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) na webu Azure Portal jako uživatel s [přístupem k fakturám.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Vybrat **faktury**
- Kliknutím **na Stáhnout fakturu** zobrazíte kopii faktury PDF. Pokud je v **části Není k** dispozici, podívejte se na informace v tématu Proč nevidím [fakturu za poslední fakturační období?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Příjem faktury v e-mailu (.pdf)**

- Na stránce [Předplatná](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) vyberte předplatné. Klikněte **na Faktury** a potom na Poslat fakturu e-mailem.
- Klikněte **na Přihlásit se k odběru** a přijměte podmínky. Budete se muset přihlásit ke každému předplatnému, které vlastníte.

Poznámka: Pokud po provedení kroků e-mail nezískáte, zkontrolujte, jestli je vaše e-mailová adresa v předvolbách komunikace [ve vašem profilu správná.](https://account.windowsazure.com/profile)

**Stažení dat o využití z portálu Azure Portal**

- Přihlaste se [do Centra účtů Azure](https://account.windowsazure.com/Subscriptions) jako správce [účtu.](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Vyberte předplatné, pro které chcete zobrazit informace o faktuře a použití.
- Vyberte **Historie fakturace.**
- Výběrem **možnosti Zobrazit aktuální** výpis zobrazíte odhad poplatků v okamžiku, kdy byl odhad vygenerován.
- Vyberte **Stáhnout využití a** stáhněte si data o denním používání jako soubor CSV. Pokud vidíte dvě dostupné verze, stáhněte si verzi 2.

Další otázky: [Navštivte dokumenty rezervované instance.](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Doporučené dokumenty**

- [Základy fakturace](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Principy použití slevy rezervované instance](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Stažení nebo zobrazení fakturační faktury Azure a dat o denním používání](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Principy použití slevy rezervované instance](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Princip využití rezervované instance pro vaše předplatné Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Princip využití rezervované instance pro registraci enterprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Náklady na software Windows, které nejsou součástí rezervovaných instancí](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervované instance v programu Partner Central Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)