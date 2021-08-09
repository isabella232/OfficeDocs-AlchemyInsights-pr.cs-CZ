---
title: 'AIP: Zásady se nechová podle očekávání'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934286"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Zásady se nechová podle očekávání

Azure Information Protection: Zásady, které se nechová podle očekávání, najdete v následujících doporučených pokynech pro různé problémy se zásadami:

1. Pokud máte problémy s vizuálními značkami, přečtěte si prosím, kdy se [používají vizuální značky](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Pokud máte problémy s automatickým označováním, přečtěte si prosím informace o tom, jak nakonfigurovat podmínky pro automatickou a doporučenou klasifikaci pro [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a Jaké typy citlivých informací [vypadají.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Pokud máte problémy s ochranou Native/Pfile, přečtěte si prosím informace o [konfiguraci rozhraní API souboru](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Zkontrolujte, jestli používáte zásady s oborem, které nejsou správně nakonfigurované: Jak nakonfigurovat zásady Azure Information Protection pro konkrétní uživatele pomocí [zásad s oborem](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Pokud automatické označování nefunguje pro Outlook při připojování označeného dokumentu, ověřte, že funkce DRMEncryptProperty není definovaná tak, jak je popsáno tady: Nastavení registru [IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)pro zabezpečení .

Pokud máte pořád problémy, shromážděte protokoly klienta Azure Information Protection a připojte exportované protokoly k tomuto lístku.

1. Otevřete dokument Office nebo vytvořte nový e-mail v Outlook.
2. Klikněte **na Zamknout/Citlivost**  >  **– nápověda a zpětná vazba.**
3. Klikněte **na Exportovat protokoly**.
4. Protokoly uložte do volby umístění a připojte je k této žádosti o službu.

Další zdroje informací:

- [Jak nakonfigurovat popisek pro vizuální označení pro Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Kontrola dokumentace k Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Použití popisků citlivosti v Microsoft 365 aplikacích](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

