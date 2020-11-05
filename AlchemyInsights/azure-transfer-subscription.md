---
title: Převod vlastnictví fakturace v Azure
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
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922029"
---
# <a name="transfer-azure-billing-ownership"></a>Převod vlastnictví fakturace v Azure

Přihlaste se k [portálu Azure](https://portal.azure.com/) jako správce fakturačního účtu, který má předplatné, které chcete přenést. Pokud si nejste jistí, jestli jste správcem, nebo pokud potřebujete zjistit, kdo je, přečtěte si článek [určení správce fakturace účtu](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Vyhledávání ve **správě nákladů + fakturace**
- Vyberte možnost **předplatná** z levého podokna. V závislosti na Accessu možná budete muset vybrat rozsah fakturace a potom **předplatné** nebo **předplatné Azure**.
- Vyberte **převést vlastnictví fakturace** pro předplatné, které chcete přenést.
- Zadejte e-mailovou adresu uživatele, který je správcem fakturace účtu, který bude novým vlastníkem předplatného, a pak vyberte **Odeslat žádost o odeslání**
- Uživatel obdrží e-mailovou zprávu s pokyny pro kontrolu žádosti o převod. Pokud chcete žádost o převod schválit, uživatel v e-mailu vybere odkaz a postupujte podle pokynů.

**Poznámka** : Pokud převedete vlastnictví svého předplatného na účet uživatele v jiném Azure AD tenantovi, budou trvale odebrány všechny úlohy [řízení přístupu založené na rolích (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)pro správu zdrojů. Jenom nový vlastník bude mít přístup ke správě zdrojů v předplatném. Další informace najdete v tématu [Převod předplatného na uživatele v jiném Azure AD tenantovi](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Doporučené dokumenty**

- [Převod vlastnictví účtu Azure na jiný účet](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [O převodu vlastnictví fakturace pro předplatné Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Přenášení Visual studia, partnera sítě Microsoft (MPN) a platby průběžně](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Časté otázky k převodu vlastnictví](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Řešení problémů s převodem vlastnictví](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
