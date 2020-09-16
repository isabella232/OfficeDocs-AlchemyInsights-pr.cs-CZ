---
title: 'AIP: zásady se nechovají podle očekávání'
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
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663182"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: zásady se nechovají podle očekávání

Azure Information Protection: zásady nefungují podle očekávání, podívejte se na následující doporučení pro různé problémy se zásadami:

1. Pokud máte problémy s vizuálními značkami, zkontrolujte, jestli [se vizuální značky používají](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Pokud máte problémy s automatickým popiskem, podívejte se [na článek Jak nakonfigurovat podmínky pro automatickou a doporučenou klasifikaci pro službu Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a [Jaké jsou tyto typy informací citlivé](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Pokud máte problémy s funkcí nativní/pfile Protection, zkontrolujte [konfiguraci rozhraní API souboru](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Zkontrolujte, jestli používáte zásady s oborem, které nejsou správně nakonfigurované: [jak nakonfigurovat zásady ochrany informací Azure pro určité uživatele pomocí zásad v oboru](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Pokud automatické připsání popisků nefunguje v Outlooku při připojování dokumentu označeného štítky, ověřte, že DRMEncryptProperty není definovaný, jak je popsáno tady: [nastavení registru IRM pro zabezpečení](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Pokud pořád dochází k problémům, Shromážděte protokoly klienta ochrany informací Azure a připojte k tomuto lístku exportované protokoly.

1. Otevřete dokument Office nebo vytvořte nový e-mail v Outlooku.
2. Klikněte na **ochrana/citlivost**  >  **a váš názor**.
3. Klikněte na **exportovat protokoly**.
4. Protokoly uložte na svůj výběr a připojte je k tomuto požadavku služby.

Další zdroje informací:

- [Jak nakonfigurovat popisek vizuálních značek pro Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Přečtěte si dokumentaci k Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Používání popisků citlivosti v aplikacích Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

