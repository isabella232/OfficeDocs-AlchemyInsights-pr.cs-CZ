---
title: Chyby při vytváření živých událostí v Yammeru
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
- "9002495"
- "5112"
ms.openlocfilehash: eb1ef3712038827beafc8eb520f9793da5f357d728e8250c16d88a99b8b5fe20
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114921"
---
# <a name="live-events-in-yammer-creation-errors"></a>Chyby při vytváření živých událostí v Yammeru

**Vytvoření živé události v Yammeru**

Yammer vždy zobrazuje možnost vytvoření živé události. V některých případech ale uživatel nemusí splňovat požadavky pro vytvoření živé události a při pokusu o její vytvoření může dojít k chybě. Níže uvedené položky popisují časté důvody pro vznik tohoto problému a poskytují způsoby jeho řešení pro koncové uživatele.

**Kdo může vytvářet živé události**
- Licence Office 365 Enterprise E1, E3 nebo E5 nebo licence Office 365 A3 nebo A5.
- Oprávnění vytvářet živé události v centru pro správu Microsoft Teams.
- Oprávnění vytvářet živé události v Microsoft Streamu (pro události produkované prostřednictvím externí vysílací aplikace nebo zařízení).
- Plné týmové členství v organizaci (nemůže to být host ani osoba z jiné organizace).
- Aktivované plánování soukromých schůzek, sdílení obrazovky a sdílení IP videa v zásadách týmových schůzek.

**Zásady vytváření živé události**

Yammer se řídí zásadami živých událostí, které jsou nastavené ve vašem tenantovi Office 365 pro Stream. Ve výchozím nastavení může živé události vytvářet kdokoli v organizaci. Správci můžou [toto nastavení změnit, což může uživatelům bránit ve vytvoření živé události](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating). V případě, že se při vytváření živé události objeví chyba zásady, je důležité zkontrolovat, jestli mají uživatelé oprávnění živé události vytvářet.
