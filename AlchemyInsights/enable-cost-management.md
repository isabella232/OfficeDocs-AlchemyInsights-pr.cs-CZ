---
title: Povolení správy nákladů
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: c3623aee9ab3592254ffb25aade7d52a2c7ddd49fde939956162cd4008d5ba19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003562"
---
# <a name="enable-cost-management"></a>Povolení správy nákladů

**Co znamená "náklady jsou pro vaši organizaci zakázané"?**

Organizace používající účty smlouva Enterprise (EA) nebo Microsoft Customer Agreement (MCA) mohou zakázat přístup k informacím o nákladech a cenám.

Po přihlášení k webu Azure Portal mohou pomocí rozhraní API pro fakturaci programově získat faktury (po přihlášení) a podrobnosti o využití.

**Jak povolit dalším uživatelům přístup k fakturám**

1. Přejděte na **Okno Předplatná na** webu Azure Portal.
2. Vyberte **Faktury a** pak Access k **fakturám**.
3. Pokud chcete uživatelům v rolích s rozsahem předplatného povolit stahování faktur, zapněte přístup a pak změny ukládáte.

> [!NOTE]
> Správce účtu taky může nakonfigurovat, aby se faktury posílaly e-mailem. Další informace najdete v tématu [Získání faktury e-mailem](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Přidání uživatelů do role Čtečka fakturace**

1. Přejděte na **Okno Předplatná na** webu Azure Portal.
2. Vyberte **Ovládací prvek Accessu (IAM)** a potom klikněte na **Přidat.**
3. Na **stránce Vybrat** **roli** zvolte Čtečka fakturace.
4. Zadejte e-mail uživatele, kterého chcete pozvat, a kliknutím na **OK** pozvánku odešlete.
5. Podle pokynů uvedených v e-mailu s pozvánkou se přihlaste jako čtečka fakturace. Další informace najdete v tématu [Udělení přístupu k fakturaci](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Doporučené dokumenty**

- [Povolení zobrazení jazyka DA a AO prostřednictvím portálu EA](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Náklady zahrnuté do správy nákladů](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Podporované Microsoft Azure nabídky](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Kontrola nákladů v analýze nákladů](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Poskytnutí přístupu k fakturačním informacím](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kontrola přístupu ke smlouvě se zákazníkem Microsoftu](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






