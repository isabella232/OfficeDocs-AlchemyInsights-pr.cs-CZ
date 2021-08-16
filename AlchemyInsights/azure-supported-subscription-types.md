---
title: Podporované typy předplatného
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
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072153"
---
# <a name="supported-subscription-types"></a>Podporované typy předplatného

Pokud chcete pokračovat dál, zkontrolujte prosím podporované typy předplatného.

[Podporované typy předplatného](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Převod vlastnictví fakturace**

Přihlaste se na portál Microsoft Azure jako [Správce fakturačního účtu](https://ms.portal.azure.com/), ke kterému je přiřazené předplatné, které chcete převést.

- Hledejte ve článku **Správa ceny + fakturace**. Vyberte **Předplatné** v levém podoknu. V závislosti na přístupu možná budete muset vybrat rozsah fakturace a poté **Předplatná** nebo **Předplatná Azure**.
- Vyberte Přenos vlastnictví fakturace u předplatného, které chcete převést.
- Zadejte e-mailovou adresu uživatele, který je správcem fakturace účtu. Ten bude novým vlastníkem předplatného. Poté vyberte možnost **odeslat požadavek na převod**.
- Tento uživatel dostane e-mail s pokyny pro kontrolu vašeho požadavku na převod. Chce-li schválit požadavek na převod, uživatel otevře odkaz v e-mailu a postupuje podle pokynů. 

Poznámka: pokud převedete vlastnictví fakturace svého předplatného na účet uživatele v jiném tenantovi Azure AD, všechna přiřazení [řízení přístupu na základě role v Azure (Azure RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) ke správě prostředků v předplatném se trvale odeberou. Ke správě zdrojů v předplatném bude mít přístup jenom jejich nový vlastník. Další informace najdete v článku [Převod předplatného na uživatele v jiném tenantovi Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Přenos vlastnictví předplatného**

Převod vlastnictví předplatného požaduje, aby přístup založený na rolích (RBAC) pro správu prostředků v předplatném přišel o přístup. Další informace o přidání existujícího předplatného tenantovi najdete v článku [Přiřazení nebo přidání předplatného Azure do tenanta Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Převod předplatného se stávající neuhrazenou částkou z aktuálního fakturačního cyklu se nepřevede na nový platební nástroj v novém účtu. Jediná informace, které je přístupná uživatelům na novém účtu, je výše vašeho předplatného za předchozí měsíc. Jiné informace týkající se historie používání a fakturace se s předplatným nepřenesou.
- Převod vlastnictví předplatného smlouvy Enterprise (EA) je aktuálně podporované jenom na portálu smlouvy Enterprise.
- Při přenosu předplatného zaměřeného na kredit, jako je například Visual Studio, BizSpark nebo Microsoft Partner Network, se vyžaduje, aby nový uživatel měl licenci k Visual Studiu / Microsoft Partner Networku, aby mohl žádost o přenos přijmout.
- Všechny prostředky, jako jsou virtuální počítače, disky a weby, se úspěšně přenesou do nového účtu. Při přenosu předplatného mezi tenanty mohou být ovlivněny následující prostředky:

**Azure AD Domain Services**

Trezory klíčů Azure

- Mohlo by to ovlivnit [Uživatele a databáze související se SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support), zejména pokud zákazník používá ověřování související s Azure Active Directory.
- Mohlo by to ovlivnit služby **App Services** nakonfigurované pomocí systému ověřování služby Azure Active Directory.
- Účty **Visual Studio Team Services** připojené k předplatným Azure můžou dočasně ztratit přístup, když se zruší připojené předplatné Azure.

**Doporučené dokumenty**

Postup po přijetí vlastnictví fakturace:

- Pokud chcete zachovat vlastnictví fakturace, ale změnit typ předplatného, přečtěte si informace v článku [Změna předplatného Azure na jinou nabídku](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support).
- [Převod vlastnictví fakturace Visual Studia, Microsoft Partner Networku (MPN) a Platby za využití pro vývoj/testování](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Převod vlastnictví fakturace předplatných smlouvy Enterprise (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Časté otázky o převodu vlastnictví](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Řešení problémů převodu vlastnictví](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)