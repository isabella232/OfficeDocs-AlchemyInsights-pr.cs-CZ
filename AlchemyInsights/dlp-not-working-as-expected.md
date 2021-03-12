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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707803"
---
# <a name="dlp-not-working-as-expected"></a>DLP nefunguje podle očekávání

**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).

 **Nastavení DLP**

Máte problémy s prevencí ztráty dat **(DLP)** v Office 365, která nefunguje podle očekávání? Pokud ano, ujistěte  se, že máte správně nastavenou zásadu  ochrany před únikem informací a jestli data obsahují to, co zásada ochrany před únikem informací hledá při vyhodnocení.
  
Zásady ochrany před únikem informací umožňují identifikovat a chránit citlivé informace ve vaší organizaci. Pokud chcete nastavit zásady ochrany před únikem informací, použijte [informace uvedené v této článku.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Jaké zásady ochrany před únikem informací hledat**
  
Při používání **integrovaných** citlivých typů informací v centrech zabezpečení a dodržování předpisů zásady ochrany před únikem informací při zjišťování těchto citlivých typů zjišťují konkrétní vzory a prvky.
  
- **Integrované citlivé typy informací**

    Informace o předdefinových typech s citlivými typy a o tom, co zásady ochrany před únikem informací hledá při zjišťování typu citlivé informace, najdete v tématu: Co citlivé typy [informací vyhledáte.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Vlastní citlivé typy informací**

    Pokud se pokoušíte vytvořit vlastní citlivé typy informací, použijte v následujícím článku informace o vytvoření vlastního citlivého typu: Vytvoření vlastního typu citlivé [informace.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Testování zásad ochrany před únikem informací**

Pokud chcete data testovat pomocí předdefinového nebo vlastního citlivého typu informací, použijte možnost **Typ** testu v části Typy informací citlivé  >  **na klasifikace.** Další informace najdete v tématu [Testování vlastních citlivých typů informací.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Sestavy**
  
- Díky sestavám ochrany před únikem informací získáte citlivé [poznatky o datech.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Podívejte se na konkrétní podrobnosti o události se [zprávou o incidentu.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
