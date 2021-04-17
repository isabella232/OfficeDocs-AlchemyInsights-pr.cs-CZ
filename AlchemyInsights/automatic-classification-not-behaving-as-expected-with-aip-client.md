---
title: Automatická klasifikace se s klientem AIP nechová podle očekávání
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
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820891"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatická klasifikace se s klientem AIP nechová podle očekávání

Automatická klasifikace se nechová podle očekávání, použijte následující doporučené pokyny:

1. Pokud máte problémy s automatickým označováním, podívejte se na postup konfigurace podmínek pro automatickou a doporučenou klasifikaci pro [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a Informace, které typy citlivých informací [vypadají.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
2. Zkontrolujte, jestli používáte zásady s oborem, které nejsou správně nakonfigurované: Jak nakonfigurovat zásady Azure Information Protection pro konkrétní uživatele pomocí [zásad s oborem](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Pokud automatické označování nefunguje v Outlooku při připojování označeného dokumentu, ověřte, jestli není definováno, jak je popsáno tady: Nastavení registru `DRMEncryptProperty` [IRM pro zabezpečení](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Pokud jste [](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) pro zásadu Azure Information Protection použili předdefinové typy informací, ověřte, že váš obsah odpovídá očekávanému formátu.
5. Ověřte, jestli je popisek správně nakonfigurovaný na **Automatické nebo** **Doporučené.** **(Automatické** označování je dostupné pro všechny aplikace Microsoft  365, zatímco doporučeno je k dispozici pro všechny aplikace Microsoft 365 s výjimkou Outlooku.)
6. Automatickou klasifikaci nelze použít u dokumentů a e-mailů, které byly dříve ručně označené nebo dříve automaticky označené vyšší klasifikací.  Další informace najdete v tématu Použití [automatických nebo doporučených štítků.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Pokud máte pořád problémy, shromážděte prosím protokoly klienta Azure Information Protection a připojte exportované protokoly k lístku podpory. Export protokolů Azure Information Protection:
    - Otevřete dokument Office nebo vytvořte nový e-mail v Outlooku.
    - Klikněte **na Zamknout/Citlivost**  >  **– nápověda a zpětná vazba.**
    - Klikněte **na Exportovat protokoly**.
    - Protokoly uložte do volby umístění a připojte je k žádosti o službu.

Další informace najdete v těchto informacích:

- [Jak nakonfigurovat podmínky pro automatickou a doporučenou klasifikaci pro Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Návody pro běžné scénáře, které používají Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Kontrola dokumentace k Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Kontrola předplatných a funkcí Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Požadavky na Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Úvodní kurz pro Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Stažení klienta Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
