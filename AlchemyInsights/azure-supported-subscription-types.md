---
title: Podporované typy předplatného
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
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807360"
---
# <a name="supported-subscription-types"></a>Podporované typy předplatného

Zkontrolujte podporované typy předplatného a pokračujte dál.

[Podporované typy předplatného](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Převést vlastnictví fakturace**

Portál Azure jako [správce účtu](https://ms.portal.azure.com/) fakturačního účtu, který má předplatné, které chcete přenést

- Vyhledávání ve **správě nákladů + fakturace** Vyberte **předplatná** z levého podokna. V závislosti na Accessu možná budete muset vybrat rozsah fakturace a potom **předplatné** nebo **předplatné Azure** .
- Vyberte převést vlastnictví fakturace pro předplatné, které chcete přenést.
- Zadejte e-mailovou adresu uživatele, který je správcem fakturace účtu, který bude novým vlastníkem předplatného, a pak vyberte **Odeslat žádost o odeslání**
- Uživatel obdrží e-mailovou zprávu s pokyny pro kontrolu žádosti o převod. Pokud chcete žádost o převod schválit, uživatel v e-mailu vybere odkaz a postupujte podle pokynů.

Poznámka: Pokud převedete vlastnictví svého předplatného na účet uživatele v jiném Azure AD tenantovi, budou trvale odebrány všechny úlohy [řízení přístupu založené na rolích (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) pro správu zdrojů. Jenom nový vlastník bude mít přístup ke správě zdrojů v předplatném. Další informace najdete v tématu [Převod předplatného na uživatele v jiném Azure AD tenantovi](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Převod vlastnictví předplatného**

Vlastnictví předplatného: přenášet přístup pomocí rolí požadavků (RBAC) pro správu prostředků v předplatném ztratí přístup. Další informace o přidání existujícího předplatného ke klientovi najdete v článku [přidružení nebo přidání předplatného Azure do služby Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Převod předplatného se stávajícím neuhrazeným množstvím z aktuálního fakturačního cyklu se nepřenese do nového platebního nástroje v novém účtu. Jedinými informacemi dostupnými pro uživatele v novém účtu je cena za poslední měsíc pro vaše předplatné. Zbývající část použití a historie fakturace se s předplatným nepřenesou.
- Převod vlastnictví účtu organizace – předplatné na základě předplatného je aktuálně podporovaný jenom na portálu Enterprise Agreement.
- Při přenosu tarifu zaměřeného na kredit, jako je třeba Visual Studio, BizSpark, musí mít Partnerská síť Microsoftu pro nového uživatele licenci pro přijetí požadavku na převod na úrovni Visual studia/Microsoft Partner Network.
- Všechny prostředky, jako virtuální počítače, disky a weby, se úspěšně přenášejí na nový účet. V přenosu předplatného mezi klienty můžou být ovlivněné tyto prostředky:

**Služby Azure AD**

Trezory klíčů Azure

- Je možné ovlivnit [uživatele a databáze související s SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) , obzvláště v případě, že zákazník používá ověřování související s Azure Active Directory.
- **Služby aplikací** nakonfigurované s ověřováním Azure Active Directory by mohly být ovlivněny
- **Visual Studio Team** Účty služeb, které jsou připojené k předplatnému Azure, můžou dočasně ztratit přístup, když je připojené předplatné Azure zrušené.

**Doporučené dokumenty**

Kroky po přijetí vlastnictví fakturace:

- Chcete-li zachovat vlastnictví fakturace, ale změnit typ svého předplatného, podívejte se na téma: [Přepnutí předplatného Azure na jinou nabídce](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support) .
- [Přenášení Visual studia, partnera sítě Microsoft (MPN) a platby průběžně](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Převést vlastnictví účtu organizace (EA) pro předplatná](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Časté otázky k převodu vlastnictví](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Řešení problémů s převodem vlastnictví](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)