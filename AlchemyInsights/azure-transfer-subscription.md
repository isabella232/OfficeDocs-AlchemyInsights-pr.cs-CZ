---
title: Převod vlastnictví fakturace Azure
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
- "6849"
ms.openlocfilehash: 454ce626862bb4a2361abccd92ad0099b534388c
ms.sourcegitcommit: 059ad2936788266ea9714ec8c66d407d7261aeb6
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/29/2020
ms.locfileid: "49736871"
---
# <a name="transfer-azure-billing-ownership"></a>Převod vlastnictví fakturace Azure

Přihlaste se na [portál Microsoft Azure](https://portal.azure.com/) jako správce fakturačního účtu s předplatným, které chcete převést. Pokud si nejste jisti, jestli jste správce, nebo potřebujete zjistit, kdo jím je, přečtěte si článek [Určování správce fakturace účtu](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Hledat na _Správa ceny + fakturace_.
1. Vyberte **Předplatné** v levém podoknu. V závislosti na přístupu možná budete muset vybrat rozsah fakturace a poté **Předplatné** nebo **Předplatné Azure**.
1. Vyberte **Přenos vlastnictví fakturace** pro předplatné, které chcete převést.
1. Zadejte e-mailovou adresu uživatele, který je správcem fakturace účtu. Ten bude novým vlastníkem předplatného. Poté vyberte možnost **odeslat požadavek na převod**.
1. Tento uživatel dostane e-mail s pokyny pro kontrolu vašeho požadavku na převod. Chce-li schválit požadavek na převod, uživatel otevře odkaz v e-mailu a postupuje podle pokynů. 

Vezměte prosím na vědomí, že pokud převedete fakturační vlastnictví svého předplatného na účet uživatele v jiném Microsoft Azure AD tenantovi, všechna přiřazení [řízení přístupu na základě rolí (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) ke správě prostředků v předplatném budou trvale odebrána. Pouze nový vlastník bude mít přístup ke správě zdrojů v předplatném. Další informace o tom, jak změnit adresář pro předplatné, najdete v článku [Převod předplatného na uživatele v jiném tenantovi Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Důležitý dopad na vaše faktury**_: pokud jste přenesli fakturační vlastnictví předplatného Azure, budou vaše poplatky poměrné. K fakturám získáte přístup následujícím způsobem:  

1. Vyberte své předplatné na stránce  [Předplatné](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)  na portálu Microsoft Azure jako  [uživatel s přístupem k fakturám](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support) a poté vyberte  **Faktury**.
1. Kopii vaší PDF faktury zobrazíte kliknutím  **Stáhnout fakturu** . Pokud se zobrazí  _Není k dispozici_, přečtěte si část [Proč nevidím fakturu za poslední fakturační období?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Můžete také zobrazit své denní využití kliknutím na **fakturační období** a získat PDF faktury a kopii vašeho souboru detailního denního použití (.CSV). Další informace najdete v  [Získání údajů o faktuře a využití](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Doporučené dokumenty**

- [Převod fakturačního vlastnictví předplatného Azure na jiný účet](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [O převodu fakturačního vlastnictví předplatného Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Převod předplatného Visual Studia, Microsoft Partner Networku (MPN) a Platby za využití pro vývoj/testování](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Časté otázky o převodu vlastnictví](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Řešení problémů převodu vlastnictví](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
