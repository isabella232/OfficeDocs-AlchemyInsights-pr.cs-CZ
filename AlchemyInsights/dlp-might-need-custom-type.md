---
title: DLP může potřebovat vlastní typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446684"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP může potřebovat vlastní typ

**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).

**DLP může vyžadovat vlastní typ informací.**

Se zásadou ochrany před únikem dat (DLP) můžete identifikovat a chránit citlivá data ve vaší organizaci. V některých situacích budete možná muset vytvořit vlastní typ citlivých informací, který bude chránit data vaší organizace. Další informace najdete v tématu [Informace o typech citlivých informací](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) a Definice entit typu Citlivé [informace](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

Další informace o tom, jak vytvořit vlastní citlivé typy informací a zásady, najdete v těchto článku: 

**Přizpůsobení integrovaného typu citlivých informací**

Pokud by předdefinový typ citlivých informací splňoval vaše potřeby pomocí několika vylepšení, podívejte se na informace v tématu Přizpůsobení [předdefinovat citlivého typu informací.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Můžete například přidat nebo odebrat klíčová slova nebo přidat nebo odebrat podpůrné důkazy, jako je datum nebo adresa.

**Vytvoření vlastního typu citlivých informací**

Pokud ale potřebujete identifikovat a zamknout úplně jiný typ citlivých informací, můžete vytvořit vlastní typ citlivých informací v Centrum dodržování předpisů Microsoftu 365. Další informace najdete v tématu [Začínáme s vlastními typy citlivých informací](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).

**Vytvoření vlastního typu citlivých informací v PowerShellu & Security & Compliance Center**

A konečně, pokud uživatelské rozhraní neposkytuje všechny možnosti, které potřebujete, můžete vytvořit vlastní typ citlivých informací v PowerShellu & Security & Compliance Center. Počínaje souborem XML můžete použít všechny dostupné možnosti. Další informace najdete v tématu [Vytvoření vlastního typu citlivých informací pomocí PowerShellu](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).

Pokud chcete nejdřív otestovat zásady v testovacím režimu, podívejte se na články Implementace zásad v [testovacím](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) režimu [a Vytvoření, testování a ladění zásad ochrany před](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy)únikem informací . 