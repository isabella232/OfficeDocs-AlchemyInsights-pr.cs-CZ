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
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080739"
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
