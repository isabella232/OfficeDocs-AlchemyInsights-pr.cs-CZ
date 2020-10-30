---
title: Proč je pro mě tlačítko Přidat rozpočet zakázané?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807216"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Proč je pro mě tlačítko Přidat rozpočet zakázané?

Chcete-li vytvořit rozpočet, potřebujete jedno z následujících oprávnění:

- Skupina pro správu, předplatné, obory skupiny prostředků
- Manažer nákladů
- Nadřazeného
- Úrovni
- Pouze podnikový zákazník: zápis, oddělení, obory účtů
- Správce registrace (nastavit rozpočet v oboru zápisu)
- Správce oddělení (nastavení rozpočtu v oboru oddělení)
- Vlastník účtu (nastavit rozpočet na obor účtu)
- Jenom moderní smlouva o zákaznících: fakturační účet, Fakturační profil, obory oddílů faktury
- Tvůrce předplatného Azure

**Vytvořili jsme rozpočet, když již překročil rozpočet na cenu za aktuální měsíc. Proč mi nepřišla upozornění?**  
Pokud jste už překročili daný limit nákladů, když vytváříte rozpočet, který se neaktivuje. Když zahájíte nový cyklus a v případě porušení prahu, bude výstraha začínat.

**Kdy mám po překročení jednoho z mých definovaných prahových hodnot výstražných výstrah očekávat upozornění?**  
Rozpočty jsou vyhodnocovány každých 4 hodin. Použití dat pro používání systému rozpočtů trvá minimálně 8 hodin. Po překročení prahu může tato výstraha trvat až 12 hodin.

**Proč je po výběru měsíce nebo období resetování fakturačního měsíce tlačítko počáteční datum zakázáno?**  
Rozpočty jsou zarovnané na aktuální kalendářní měsíc nebo aktuální fakturační období (v případě, že je vybrán měsíc fakturace). Proto tuto hodnotu zadáme předem.

**Proč se v průběhu tvorby rozpočtu nezobrazuje graf mých nákladů?**  
Před vykreslením grafu, který vám pomůže s vytvářením rozpočtu, potřebujeme minimálně 2 měsíce.

**Proč nemohu nastavit rozpočet na základě předplatného, které jsem vytvořil (a)?**  
Po vytvoření předplatného trvá zpracování dat 24-48 hodin před nastavením rozpočtu.

**Prostředky API rozpočtu**

- [Rozpočty API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): poskytuje operace vytváření a aktualizace rozpočtů. Pomocí rozhraní API rozpočtů můžete nastavit práh rozpočtu a nakonfigurovat více výstrah tak, aby se požárly při přístupu k této prahové hodnotě. Upozornění můžou aktivovat e-mail nebo skupinu akcí Azure, která provádí automatizaci. Poznámka: filtrování tohoto rozhraní API se nerovná s filtrováním nebo rozměry rozhraní API pro dotazy.
- [Rozpočtová rozhraní API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Vytvořte rozpočty s funkcemi filtrování většího nákladu než v1. Filtrování se zarovná se smlouvou použitým v rozhraní API dotazu a dimenze. Toto je doporučená rozpočtová rozhraní API pro použití přesunutí dopředu.
- [Dimenze](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): poskytuje operace pro dosažení podporovaných dimenzí pro použití v různých oborech. Pomocí rozhraní API Dimensions můžete načíst seznam dimenzí, které můžete použít jako vstupy pro generování dotazů pomocí rozhraní API dotazu.
- [Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): umožňuje operacím získat agregované údaje o nákladech a využití založené na dotazu, který jste zadali. Pomocí rozhraní API dotazu můžete určit požadované filtrování, řazení a seskupování podle dostupných dimenzí (které jsou přístupné z rozhraní API pro dimenze).

**Předpokládané náklady**

**Proč nevidím předpovědi pro náklady na analýzu nákladů?**  
Existuje několik důvodů, proč může být prognóza předpovědi pro vás při analýze nákladů chybná, některé z nich jsou následující:

1. Pokud jsou údaje o nákladech starší než 10 dní, nebude graf prognózy zaveden. Model vyžaduje nejméně 10 dní nedávných údajů o nákladech pro přesné výčnělky.
2. Pokud jste vybrali historické kalendářní data, nebude graf prognózy viditelný. Vyberte rozsah kalendářních dat s budoucími kalendářními daty pro graf prognózy.
3. Pokud má váš účet více měn, graf prognózy bude projektovat pouze za ' všechny náklady v USD '.

**Proč se při změnách mých zdrojů nemění prognóza?**  
Model prognózy vyžaduje pro změny v účtu několik dnů a neumožňuje okamžité výčnělky založené na změnách zdrojů.  
V případě větších kroků zvýšení nebo snížení zdrojů bude mít model na tyto změny v případě anomálií na nepravidelnosti déle.

**Proč se prognóza zvýší po provedení rezervace nebo zakoupení tržiště?**  
Model prognózy má za to, že se jedná o skutečné náklady a nepoužívá se k žádnému nákupu. V případě jednorázového nákupu model sníží náklady po 10 dnech k náhlému zvýšení nákladů.

**Chci zobrazit prognózy pro jednu dimenzi (např. Ukazatel**  
Prognóza aktuálně podporuje celkové nákladové prognózy a ne pro jednotlivé plynoměry. Proto když ' seskupeno podle ' dimenze, budou celkové výčnělky celkem všechny položky v dimenzi

**Doporučené dokumenty**

- [Co je Správa nákladů Azure?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Osvědčené postupy pro řízení nákladů Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analýza nákladů a výdajů](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Zkoumání a analýza nákladů pomocí analýzy nákladů](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Správa nákladů Azure: ceny](https://azure.microsoft.com/services/cost-management/#pricing)
- [Zkontrolovat náklady v analýze nákladů](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video kurz: vytvoření rozpočtu na portálu Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Předpoklady pro zobrazení a přizpůsobení rozpočtů](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Vytváření a Správa rozpočtů](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurace automatizace pomocí skupin akcí a rozpočtů Azure](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Použití oznámení o nákladech ke sledování využití a výdajů](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Doporučené postupy pro řízení nákladů](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Výuková videa**

- [Vytvoření rozpočtu na portálu Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Správa nákladů pomocí API rozpočtů a skupin akcí](https://go.microsoft.com/fwlink/?linkid=2147038)