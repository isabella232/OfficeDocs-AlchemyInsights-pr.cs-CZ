---
title: Proč je tlačítko Přidat rozpočet pro mě zakázané?
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
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954657"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Proč je tlačítko Přidat rozpočet pro mě zakázané?

Pokud chcete vytvořit rozpočet, potřebujete jedno z následujících oprávnění:

- Skupina pro správu, předplatné, obory skupin prostředků
- Přispěvatel správy nákladů
- Vlastník
- Přispěvatel
- Enterprise Pouze zákazník: Registrace, oddělení, obory účtů
- Správce registrace (nastavte rozpočet na obor Registrace)
- Správce oddělení (nastavit rozpočet na obor oddělení)
- Vlastník účtu (nastavit rozpočet na rozsah účtu)
- Pouze moderní zákaznická smlouva: Fakturační účet, Fakturační profil, Rozsahy oddílu faktury
- Tvůrce předplatného Azure

**Rozpočet jsem vytvořil(a), když moje náklady na aktuální měsíc už byly nadrozpočtové. Proč jsem neobdržel(a) upozornění?**  
Pokud jste už překročili danou prahovou hodnotu nákladů při vytváření rozpočtu, který upozornění nevyhodí. Jakmile začne nový cyklus, pokud mezní hodnotu porušíte, výstraha se spustí.

**Kdy mám očekávat, že po překročení jedné z definovaných mezních hodnot upozornění na rozpočet obdržím upozornění?**  
Rozpočty se vyhodnocují každé 4 hodiny. Než se data o využití dostanou do rozpočtového systému, trvá minimálně 8 hodin. Vzhledem k tomu může po překročení mezní hodnoty trvat upozornění až 12 hodin.

**Proč je tlačítko Počáteční datum zakázané, když vyberu období resetování měsíce nebo fakturačního měsíce?**  
Rozpočty jsou zarovnané k aktuálnímu kalendářnímu měsíci nebo aktuálnímu fakturačnímu období (v případě, že je vybraný fakturační měsíc). Proto tuto hodnotu předplňujeme za vás.

**Proč nevidím graf nákladů v prostředí vytváření rozpočtu?**  
Než vykreslíme graf, který vám pomůže s vytvářením rozpočtu, potřebujeme minimálně 2 měsíce nákladových dat.

**Proč nemůžu nastavit rozpočet na předplatné, které jsem právě vytvořil(a)?**  
Po vytvoření předplatného trvá zpracování dat 24–48 hodin, než se na něj nastaví rozpočet.

**Zdroje rozhraní API pro rozpočet**

- [Budgets API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Poskytuje operace pro vytváření a aktualizaci rozpočtů. Pomocí rozhraní Budgets API můžete nastavit prahovou hodnotu rozpočtu a nakonfigurovat několik upozornění tak, aby se přiblíží této mezní hodnotě. Výstrahy mohou aktivovat e-mail nebo skupinu akcí Azure k provedení automatizace. Poznámka: Filtrování pro toto rozhraní API není v souladu s filtrováním a rozměry rozhraní Api dotazů.
- [Rozhraní Budgets API v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)Vytvářejte rozpočty s vyššími možnostmi filtrování nákladů než v1. Filtrování zarovná smlouvu použitou v našich rozhraních API pro dotazy a rozměry. Toto je doporučené rozhraní API rozpočtů, které se používá k přechodu kupředu.
- [Rozměry:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Poskytuje operace pro získání podporovaných rozměrů pro vaše použití v různých oborech. Pomocí rozhraní Dimensions API můžete načíst seznam dimenzí, které se používají jako vstupy pro generování dotazů pomocí rozhraní Query API.
- [Dotaz:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Poskytuje operace pro získání agregovaných dat o nákladech a využití na základě dotazu, který dodáte. Pomocí rozhraní Query API můžete zadat požadované filtrování, řazení a seskupování na všech dostupných dimenzích (které jsou přístupné z rozhraní Dimensions API).

**Předpovídá se náklady**

**Proč nevidím prognózy nákladů v analýze nákladů?**  
V analýze nákladů může prognóza chybět z několika důvodů, některé z nich jsou následující:

1. Pokud jsou data nákladů kratší než 10 dní, graf prognózy se nenačte. Model vyžaduje minimálně 10 dní posledních nákladových dat pro přesné projekce.
2. Pokud jste vybrali historická data, graf prognózy se nezobrazí. Vyberte rozsah dat s budoucími daty pro zobrazení prognózového grafu.
3. Pokud má váš účet více měn, bude v předpovídce pouze projektové náklady na "Všechny náklady v USD".

**Proč se prognóza nezmění, když změním svoje zdroje?**  
Model prognózy vyžaduje pár dní, aby se zohlednily změny v účtu a nepromítly okamžité prognózy založené na změně zdrojů.  
U větších kroků zvýšení nebo snížení zdrojů bude model trvat o něco déle, než se přizpůsobí těmto změnám, aby se zohlednily anomálie.

**Proč se moje prognóza po provedení rezervace nebo nákupu na Marketplace zvyšuje?**  
Model prognózy bere v úvahu vaše skutečné náklady a nezahrnuje použití a nákup zvlášť. U jednoho nákupu model sníží prognózy po 10 dnech, aby se zohlednily náhlý nárůst nákladů.

**Chci zobrazit prognózy pro jednu dimenzi (např. Metr)**  
Prognóza v současné době podporuje celkové prognózy nákladů a ne pro jednotlivé metry. Pokud tedy rozměr seskupíte podle, budou projekce součet všech položek v dimenzi.

**Doporučené dokumenty**

- [Co je Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Osvědčené postupy pro Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analýza nákladů a výdajů](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Prozkoumání a analýza nákladů pomocí analýzy nákladů](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Ceny](https://azure.microsoft.com/services/cost-management/#pricing)
- [Kontrola nákladů v analýze nákladů](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Instruktážní video: Vytvoření rozpočtu na portálu Azure Portal](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Předpoklady pro zobrazení a přizpůsobení rozpočtů](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Vytváření a správa rozpočtů](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurace automatizace pomocí rozhraní Api pro skupiny akcí a rozpočty Azure](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Sledování využití a výdajů pomocí upozornění na náklady](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Doporučené postupy pro správu nákladů](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Výuková videa**

- [Vytvoření rozpočtu na portálu Azure Portal](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Správa nákladů pomocí rozhraní API rozpočtů a skupin akcí](https://go.microsoft.com/fwlink/?linkid=2147038)