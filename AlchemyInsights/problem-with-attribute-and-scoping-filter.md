---
title: Problém s atributem a filtrem rozsahu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481099"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problém s atributem a filtrem rozsahu

**Problém s konfliktním hodnotami UPN**

The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique.** Operace se nezdařila, protože hodnota celého ovládacího název uživatele (UPN) zadaná pro přidání nebo úpravy není jedinečná v celé doménové struktuře. Podrobnosti chyby: **CONSTRAINT_ATT_TYPE - userPrincipalName.**

Hodnota **userPrincipalName,** která se snaží nastavit konektor Workday při vytváření uživatelského účtu služby AD, už v cílové doméně služby AD existuje. Znamená to, že některý (1) uživatel už existuje a odpovídající kontrola ID se pro uživatele nezdařila, nebo (2) pravidlo generování upn vygeneroval konfliktní hodnotu.

Tady jsou navrhované kroky řešení:

Pokud už uživatel existuje a odpovídající kontrola ID se nepovedlo propojit účet Workday s účtem Active Directory, zkontrolujte, jestli odpovídající atribut ID (obvykle ID **zaměstnance)** v workday i AD obsahuje přesnou shodu. Pokud se neshodují, je to problém s daty, který je potřeba opravit. Pokud je třeba ID zaměstnance v pracovní den 001052 a v ad je 1052, modul zřizování tyto dva účty nepropojí a pokusí se vytvořit uživatele, který už existuje. Řešením v tomto případě je změnit hodnotu **ID** Zaměstnance v ad tak, aby zahrnovala počáteční nuly na 001052.
Pokud výraz, který generuje hlavní název uživatele, negeneruje jedinečnou hodnotu, zvažte možnost použít funkci **SelectUniqueValue** deplikace, která pokaždé vygeneruje jedinečnou hodnotu.

**U uživatelského účtu služby AD Workday se nenastaví hodnota atributu správce pro uživatelský účet služby AD.**

Úloha Workday to AD User Provisioning nenastavuje hodnotu **atributu správce** pro uživatelské účty služby AD. Existují dva možné scénáře, kdy se toto chování zobrazí:

1. Vedoucího v pracovní dny nelze rozpoznat na odpovídající uživatelský účet služby AD, protože nad rámec nemá.
2. Ve **scénáři s víc** doménami ad není vedoucí v pracovní dny ve stejné doméně jako uživatel.

Zkuste tento problém vyřešit pomocí následujících kroků:

1. Pokud jste definovali filtry rozsahu, nejdřív zkontrolujte, jestli vedoucí má obor a jestli splňuje klauzuli pro vymezení rozsahu. Pokud manažer filtr oboru nesplňuje, změňte filtr tak, aby vedoucí byl také v rozsahu operace zřizování.
2. Pokud máte víc domén AD, má spojnice známé omezení, že se neřeší odkazy na správce křížových domén.

Další podrobnosti o konfiguraci pracovního dne pro automatické zřizování najdete v kurzu: Konfigurace [funkce Workday pro automatické zřizování uživatelů.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)













