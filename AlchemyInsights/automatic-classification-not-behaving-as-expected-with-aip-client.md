---
title: Automatická klasifikace se u klienta AIP nechová očekávaným způsobem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 8c79ab50e7ddbda0cf61eb9a95279f6c42cc515c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581188"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatická klasifikace se u klienta AIP nechová očekávaným způsobem

Automatická klasifikace se nechová podle očekávání, použijte následující doporučené pokyny:

1. Pokud máte problémy s automatickým popisováním, přečtěte [si přečtěte si postup konfigurace podmínek pro automatickou a doporučenou klasifikaci pro Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a co [vyhledávají typy citlivých informací](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Zkontrolujte, jestli používáte zásady s vymezeným oborem, které nejsou správně nakonfigurovány: [Jak nakonfigurovat zásady Ochrany informací Azure pro konkrétní uživatele pomocí zásad s vymezeným oborem](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Pokud automatické popisování nefunguje pro Aplikaci Outlook při připojování dokumentu s popiskem, ověřte, že `DRMEncryptProperty` není definován, jak je popsáno zde: [Nastavení registru IRM pro zabezpečení](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Pokud jste pro zásady ochrany informací Azure použili [předdefinované typy informací,](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) ověřte, zda obsah odpovídá očekávanému formátu.
5. Ověřte, zda je popisek správně nakonfigurován pro **možnost Automatické** nebo **Doporučené**. **(Automatické** označování je k dispozici pro všechny aplikace Microsoft 365, zatímco **doporučené** je k dispozici pro všechny aplikace Microsoft 365 s výjimkou aplikace Outlook.)
6. Pro dokumenty a e-maily, které byly dříve ručně označeny nebo dříve automaticky označeny vyšší klasifikací, nelze použít automatickou klasifikaci.  Další informace naleznete v tématu: [Způsob použití automatických nebo doporučených popisků](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Pokud stále dochází k problémům, shromažďovat protokoly klientů Azure Information Protection a připojit exportované protokoly k lístku podpory. Export protokolů Azure Information Protection:
    - Otevřete dokument Office nebo vytvořte nový e-mail v Outlooku.
    - Klepněte na tlačítko **Chránit/citlivost**  >  **nápovědy a zpětné vazby**.
    - Klepněte na **položku Exportovat protokoly**.
    - Uložte protokoly do svého výběru umístění a připojte je k žádosti o službu.

Další informace naleznete v tématu:

- [Konfigurace podmínek pro automatickou a doporučenou klasifikaci pro Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Návody pro běžné scénáře, které používají Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Kontrola dokumentace ochrany informací Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Kontrola předplatných a funkcí Ochrany informací Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Požadavky na azure information protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Úvodní kurz pro Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Stažení klienta Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
