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
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679686"
---
# <a name="dlp-not-working-as-expected"></a>DLP nefunguje podle očekávání

**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).

 **Nastavení DLP**

Máte potíže s **zabráněním ochrany dat (DLP)** v Office 365 nefunguje podle očekávání? Pokud ano, ujistěte se, že máte správně nastavené **Zásady ochrany před únikem informací** a že vaše data obsahují informace o tom, co při vyhodnocování **Zásada ochrany před úniky** hledá.
  
Zásady ochrany před únikem umožňuje identifikovat a chránit citlivé informace ve vaší organizaci. K nastavení zásad ochrany před únikem informací použijte [tyto informace.](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)
  
 **Co vyhledává zásady ochrany před únikem**
  
Při používání **vestavěných citlivých informací** v centru zabezpečení a dodržování předpisů vyhledává zásady pro DLP při zjišťování těchto citlivých typů určité vzorky a prvky.
  
- **Předdefinované citlivé typy informací**

    Informace o vestavěných citlivých typech a o tom, co zásada ochrany před úniky hledá při zjišťování citlivého typu, najdete v tématu: [Jaké typy citlivých informací vypadají](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Vlastní typy citlivých informací**

    Pokud chcete vytvořit vlastní typy citlivých informací, použijte následující článek, kde najdete informace o tom, jak vytvořit vlastní typ citlivých informací: [Vytvořte si vlastní typ citlivých informací](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testování zásad ochrany před únikem informací**

Chcete-li testovat data pomocí předdefinovaných nebo vlastních typů citlivých informací, použijte možnost **Typ testu** **v části**  >  **typy utajovaných informací**. Další informace najdete v článku [testování vlastních typů citlivých informací](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Sestavy**
  
- Získejte citlivé datové přehledy s informacemi o [DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Podívejte se na určité podrobnosti o události se [sestavou incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
