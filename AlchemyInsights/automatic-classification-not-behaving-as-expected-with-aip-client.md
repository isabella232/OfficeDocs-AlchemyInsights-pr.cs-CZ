---
title: Automatická klasifikace se nechová podle očekávání klienta AIP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: d7a2246d78cbd6c4ab40c2a4e5a21807933b619a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715194"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatická klasifikace se nechová podle očekávání klienta AIP

Automatická klasifikace nefunguje podle očekávání, použijte následující doporučené pokyny:

1. Pokud máte problémy s automatickým popiskem, podívejte se [na článek Jak konfigurovat podmínky pro automatickou a doporučenou klasifikaci pro službu Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a [Jaké jsou tyto typy informací citlivé](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Zkontrolujte, jestli používáte zásady s oborem, které nejsou správně nakonfigurované: [jak nakonfigurovat zásady ochrany informací Azure pro určité uživatele pomocí zásad v oboru](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Pokud automatické připsání popisků nefunguje v Outlooku při připojování dokumentu označeného štítky, ověřte, jestli `DRMEncryptProperty` není definované tady: [nastavení registru IRM pro zabezpečení](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Pokud jste pro zásady ochrany informací Azure používali [předdefinované typy informací](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) , zkontrolujte, jestli váš obsah odpovídá očekávanému formátu.
5. Ověřte, že je popisek správně nakonfigurovaný pro **Automatické** nebo **Doporučené**. (**Automatické** popisování je k dispozici pro všechny aplikace Microsoft 365, zatímco **Doporučené** jsou pro všechny aplikace Microsoft 365 s výjimkou Outlooku.)
6. U dokumentů a e-mailů, které byly dříve označené nebo automaticky označené vyšší klasifikací, nemůžete použít automatickou klasifikaci.  Další informace najdete v tématu: použití [automatických nebo doporučených popisků](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Pokud pořád dochází k problémům, Shromážděte protokoly klienta ochrany informací Azure a připojte exportované protokoly k lístku podpory. Export protokolů ochrany informací Azure:
    - Otevřete dokument Office nebo vytvořte nový e-mail v Outlooku.
    - Klikněte na **ochrana/citlivost**  >  **a váš názor**.
    - Klikněte na **exportovat protokoly**.
    - Protokoly uložte na svůj výběr a připojte je k žádosti o služby.

Další informace najdete v těchto tématech:

- [Konfigurace podmínek pro automatickou a doporučenou klasifikaci pro službu Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Návody pro běžné scénáře používající službu Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Přečtěte si dokumentaci k Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Přečtěte si předplatné a funkce služby Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Požadavky na ochranu informací Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Rychlý kurz pro rychlé zahájení ochrany informací Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Stáhnout klienta ochrany informací v Azure](https://www.microsoft.com/download/details.aspx?id=53018)
