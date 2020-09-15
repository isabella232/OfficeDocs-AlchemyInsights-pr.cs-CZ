---
title: Vytvoření veškerého e-mailového catch
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
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712979"
---
# <a name="create-an-email-catch-all"></a>Vytvoření veškerého e-mailového catch

Důrazně se nedoporučuje použít veškerý úlovek. Je lepší poskytnout odesilateli zpátky, kteří mu odešlou vědět, že nemohly být doručeny, aby mohli dělat žádné kroky. Sledovanou poštovní schránku můžete také omezit tak, aby bylo možné zachytit dříve platné e-mailové adresy. 

Všechny úlovky budou dostávat dobré věci nevyžádané pošty a mohou nakonec plnit případné Nesledované. (Existují limity.) 

Pokud se rozhodnete pokračovat, postupujte takto:

1. Vytvořte dynamickou distribuční skupinu & zahrnout "všechny typy příjemců".

2. Vytvořte vyhrazenou poštovní schránku pro zachycování e-mailů, například catchall@domain.com.

3. Pro určitou doménu nastavte DomainType na "InternalRelay". Pokud později zachytíte celý úlovek, nastavte doménu zpět na hodnotu autoritativní.

4. Vytvořte – Poštyhttps://Configure.Office.com/Scenario.aspx?SID=12:

    - Pokud je odesílatel "mimo organizaci"
    - Přesměrovat zprávu na Catchall@domain.com
    - Kromě případu, kdy je příjemce členem allusers@domain.com (distribuční skupina obsahuje všechny členy)
    - Ověření, že nové poštovní schránky se přidají do dynamické distribuční skupiny
