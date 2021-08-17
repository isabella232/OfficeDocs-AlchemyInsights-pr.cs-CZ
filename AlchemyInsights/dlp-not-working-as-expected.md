---
title: DLP nefunguje podle očekávání
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079695"
---
# <a name="dlp-not-working-as-expected"></a>DLP nefunguje podle očekávání

**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).

 **Nastavení DLP**

Máte problémy s prevencí ztráty dat **(DLP)** v Office 365 nefunguje očekávaným způsobem? Pokud ano, ujistěte  se, že máte správně nastavené zásady ochrany před únikem informací a že data obsahují to, co při vyhodnocení zásady **ochrany** před únikem informací hledá.
  
Zásady ochrany před únikem informací umožňují identifikovat a chránit citlivé informace ve vaší organizaci. Pokud chcete nastavit zásady ochrany před únikem informací, použijte informace [tady](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).
  
 **Jaké zásady ochrany před únikem informací vypadají**
  
Při použití **předdefinované** citlivé typy informací v centrech zabezpečení a dodržování předpisů zásady DLP při zjišťování těchto citlivých typů zjišťují konkrétní vzory a prvky.
  
- **Předdefinové typy citlivých informací**

    Informace o předdefinových citlivých typech a o tom, co zásady ochrany před únikem informací vyhledá při zjišťování typu Citlivé, najdete v tématu: Co tyto typy citlivých [informací vyhledá.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Vlastní typy citlivých informací**

    Pokud se pokoušíte vytvořit vlastní citlivé typy informací, použijte následující článek s informacemi o tom, jak vytvořit vlastní citlivý [typ: Vytvoření vlastního](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)typu citlivých informací .

**Testování zásad ochrany před únikem informací**

Pokud chcete otestovat data pomocí předdefinového nebo vlastního typu citlivých informací, použijte možnost **Typ** testu v **části Klasifikační**  >  **typy citlivých informací**. Další informace najdete v tématu [Testování vlastních citlivých typů informací](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Sestavy**
  
- Získejte citlivé poznatky o datech pomocí [sestav DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Konkrétní podrobnosti o události najdete v hlášení [o incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
