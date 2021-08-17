---
title: Fakturace zakoupení služby Reserved Instance
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
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104013"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fakturace zakoupení služby Reserved Instance

Nákup rezervované instance se bude účtovat podle způsobu platby spojeného s předplatným, který si vyberete při platbě. Typ předplatného musí být smlouva Enterprise (číslo nabídky: MS-AZR-0017P), průběžné platby (číslo nabídky: MS-AZR-0003P), Smlouva se zákazníkem Microsoftu nebo CSP.

- V případě předplatného pro podniky se poplatky odečtou ze zůstatku peněžního závazku nebo se účtují jako nadlimitní využití.
- U předplatného typu průběžných plateb se vám účtují poplatky za platbu platební kartou nebo fakturou.

**Zrušení rezervace**

- **Samoobslužné funkce:** Rezervované instance můžete sami zrušit nebo vyměnit přes [portál Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vyberte rezervaci a klikněte na refundaci nebo výměnu. Upozorňujeme, že pro výměnu nebo refundaci musíte mít přístup vlastníka k objednávce rezervace. Přístup jenom k rezervacím vám neumožní pokračovat v refundaci nebo výměně. Požádejte vlastníka objednávky rezervace, aby vám k ní dal přístup.
- **Zásady výměny:** Rezervaci můžete vyměnit za jinou rezervaci stejného typu – za výměnu rezervace **nebudete penalizováni**. Celkový závazek nové rezervace by měl být vyšší než součet refundované částky vyměněné rezervace a budoucích měsíčních plateb (v příslušných případech).
- **Zásady refundace:** Součet refundované částky a zrušených budoucích plateb nesmí ve 12 kalendářních měsících překročit 50 000 USD. **Momentálně refundace nepenalizujeme**, což se ale v budoucnu může změnit.

**Výjimky:** Samoobslužná výměna a zrušení nejsou dostupné zákazníkům smlouvy Enterprise ve státní správě USA.

- Podpora pro **API/PS/CLI** není dostupná pro zrušení a refundace. [Samoobslužné výměny a refundace za rezervace Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Samoobslužná výměna a zrušení nejsou dostupné zákazníkům smlouvy Enterprise ve státní správě USA. Podporované jsou jiné typy předplatného státní správy USA, včetně platby typu průběžná platba a CSP.

Další informace : [Zpracování transakcí](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) vrácení a výměny Další informace : [Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) a Zásady refundace Další otázky: Navštivte dokumenty [rezervované instance](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Výměna existující rezervované instance (samoobslužná funkce)**

Rezervaci můžete vyměnit za jinou rezervaci stejného typu. Rezervaci můžete refundovat do výše 50 000 USD ročně, pokud už ji nepotřebujete. Samoobslužná výměna a zrušení nejsou dostupné zákazníkům smlouvy Enterprise ve státní správě USA. Podporované jsou jiné typy předplatného státní správy USA, včetně platby typu průběžná platba a CSP. Pro výměnu nebo refundaci existující rezervace musíte mít přístup vlastníka k objednávce rezervace.

Následující kroky vás provedou postupem pro dokončení transakce.

1.Přihlaste se k [portálu Azure Portal.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Vyberte rezervace, které chcete vrátit, a klikněte na **Exchange** 2.Vyberte produkt virtuálního počítače, který chcete koupit, a zadejte množství. Ujistěte se, že nový nákupní součet je víc než celkový výnos. Před nákupem určete [správnou velikost.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Zkontrolujte a dokončete transakci.

**Refundace za rezervovanou instanci**

Pokud chcete refundovat rezervaci, přejděte na **Podrobnosti rezervace** a klikněte na možnost **Refundace**.

**Poměrná refundace:**

Pro a minimálních požadavků **pro refundaci a výměnu** Příklad rezervace předem:

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

**Fakturu za poslední fakturační období se nepodařilo zobrazit.**

Některé možné důvody, proč se vám faktura nemusí zobrazit:

- U předplatného máte měsíční kredit, který jste nepřekročili nebo máte bezplatnou zkušební verzi. Faktura se vygeneruje jenom v případě, že jste dlužní peníze.
- Je to méně než 30 dní ode dne, kdy jste se přihlásili k odběru Azure.
- Faktura se ještě nevygeneruje. Počkejte až do konce fakturačního období.
- Pokud nejste správcem účtu, starší faktury nemusí být pro vás dostupné.

**Stáhněte si fakturu z webu Azure Portal (.pdf)**

- Vyberte předplatné na stránce [Předplatná](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) na webu Azure Portal jako uživatel s [přístupem k fakturám.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Vybrat **faktury**
- PDF kopii své faktury zobrazíte kliknutím na **Stáhnout fakturu**. Pokud se zobrazí **Není k dispozici**, přečtěte si část [Proč se mi nezobrazuje faktura za poslední fakturační období?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Příjem faktury e-mailem (.pdf)**

- Na stránce [Předplatná](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) vyberte předplatné. Klikněte **na Faktury** a potom na Poslat fakturu e-mailem.
- Klikněte **na Přihlásit se k odběru** a přijměte podmínky. Budete se muset přihlásit ke každému předplatnému, které vlastníte.

Poznámka: Pokud po provedení kroků e-mail nezískáte, zkontrolujte, jestli je vaše e-mailová adresa v předvolbách komunikace [ve vašem profilu správná.](https://account.windowsazure.com/profile)

**Stažení dat o využití z portálu Azure Portal**

- Přihlaste se [do Centra účtů Azure](https://account.windowsazure.com/Subscriptions) jako správce [účtu.](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Vyberte předplatné, pro které chcete zobrazit informace o faktuře a použití.
- Vyberte **Historie fakturace.**
- Výběrem **možnosti Zobrazit aktuální** výpis zobrazíte odhad poplatků v okamžiku, kdy byl odhad vygenerován.
- Vyberte **Stáhnout využití a** stáhněte si data o denním používání jako soubor CSV. Pokud vidíte dvě dostupné verze, stáhněte si verzi 2.

Další otázky: [Podívejte se na dokumenty o rezervovaných instancích](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Doporučené dokumenty**

- [Základy fakturace](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Principy použití slevy rezervované instance](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Stažení nebo zobrazení fakturační faktury Azure a dat o denním používání](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Principy použití slevy rezervované instance](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Princip využití rezervované instance pro vaše předplatné Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Princip využití rezervované instance pro registraci Enterprise instancí](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows softwaru, které nejsou součástí rezervovaných instancí](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervované instance v centrálním partnerském Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)