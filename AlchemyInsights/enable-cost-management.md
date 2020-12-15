---
title: Povolit správu nákladů
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
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676958"
---
# <a name="enable-cost-management"></a>Povolit správu nákladů

**Co znamená, že náklady jsou pro vaši organizaci zakázané?**

Organizace používající podnikové smlouvy (EA) nebo účty Microsoft Customer Agreement (MCA) mohou zakázat přístup k informacím o nákladech a cenách.

Po přihlášení k Azure Portal mohou používat API pro fakturaci k programovému získávání faktur (po obdržení) a podrobností o využití.

**Jak povolit dalším uživatelům přístup k fakturám**

1. Přejděte na **okno předplatná** na portálu Azure.
2. Vyberte **faktury** a pak **přístup k fakturám**.
3. Zapnutím Accessu a uložením změn umožníte uživatelům v rolích s rozsahem předplatného stáhnout faktury.

> [!NOTE]
> Správce účtu může také nakonfigurovat, aby faktury poslal e-mailem. Další informace najdete v tématu [získání faktury v e-mailu](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Přidání uživatelů do role čtečka fakturace**

1. Přejděte na **okno předplatná** na portálu Azure.
2. Vyberte **řízení přístupu (IAM)** a potom klikněte na **Přidat**.
3. Na stránce **Vybrat roli** zvolte **čtečka fakturace** .
4. Zadejte e-mail uživatele, kterého chcete pozvat, a kliknutím na **OK** pozvánku odešlete.
5. Postupujte podle pokynů v e-mailu pozvat pro přihlášení jako čtečku fakturace. Další informace najdete v článku [udělení přístupu k fakturaci](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Doporučené dokumenty**

- [Povolení zobrazení DA a AO na portálu EA](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Náklady zahrnuté v řízení nákladů](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Podporované nabídky Microsoft Azure](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Zkontrolovat náklady v analýze nákladů](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Poskytnutí přístupu k fakturačním informacím](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kontrola přístupu ke Smlouvě o zákaznících Microsoftu](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






