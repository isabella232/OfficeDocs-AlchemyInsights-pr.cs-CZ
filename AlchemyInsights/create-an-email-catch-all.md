---
title: Vytvoření e-mailu zachyťte vše
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816193"
---
# <a name="create-an-email-catch-all"></a>Vytvoření e-mailu zachyťte vše

Použití všech úlovek se důrazně nedoporučuje. Je lepší vrátit odesílateli zprávu, která odesílatelům umožní zjistit, že jejich zprávu nelze doručit jako adresu, aby mohli provést akci. Monitorovanou poštovní schránku můžete omezit jenom na zachycení dříve platných e-mailových adres. 

Každá poštovní schránka, která zachytí všechny poštovní schránky, dostane hodně spamu a může se vyplnit, pokud není pečlivě sledována. (Existují limity příjmu.) 

Pokud se rozhodnete pokračovat, postupujte takto:

1. Vytvořte dynamickou distribuční skupinu, & "Všechny typy příjemců".

2. Vytvořte vyhrazenou poštovní schránku pro zachycení e-mailů, například catchall@domain.com.

3. Pro konkrétní doménu nastavte Typ_domény na "InternalRelay". Pokud později odeberete všechny zachytáky, nezapomeňte doménu nastavit zpátky na Autoritativní.

4. Vytvořte pravidlo přenosu pošty takto:

    - Pokud je odesílatel mimo organizaci
    - Přesměrovat zprávu na Catchall@domain.com
    - S výjimkou případu, kdy je příjemce členem allusers@domain.com (distribuční skupina obsahuje všechny členy)
    - Ujistěte se, že se nové poštovní schránky přidávají do dynamické distribuční skupiny.
