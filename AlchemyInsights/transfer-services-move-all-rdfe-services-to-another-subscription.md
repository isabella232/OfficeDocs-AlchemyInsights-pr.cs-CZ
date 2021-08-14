---
title: Přenos služeb – přesunutí všech služeb RDFE do jiného předplatného
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940031"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Přenos služeb – přesunutí všech služeb RDFE do jiného předplatného

**Přesunutí zdrojů**

Prostředky Azure můžete přesunout do jiného předplatného Azure nebo skupiny prostředků v rámci stejného předplatného pomocí portálu Azure Portal, Azure PowerShell, Rozhraní příkazového řádku Azure nebo rozhraní REST API k přesunutí prostředků.

Než budete moci přesunout zdroje, podívejte se na:

- [Kontrolní seznam před přesunutím zdrojů](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Služby, které je možné přesunout](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Jak ověřit přesunutí](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Pokyny k přesunutí služeb](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Pokud chcete přesunout existující zdroje do jiné skupiny prostředků nebo předplatného, můžete použít:

- [Portál Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Kurz: [Přesunutí prostředků Azure do jiné skupiny prostředků nebo předplatného](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Poradce při potížích s Azure Resource Managerem**

V následujících článcích se dozvíte o některých běžných chybách nasazení Azure a obdržíte informace, které je vyřeší. Pokud nemůžete najít kód chyby pro chybu nasazení, podívejte se na informace v [tématu Vyhledání kódu chyby](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Poradce při potížích s nasazením](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Řešení potíží s přesunutím prostředků Azure do nové skupiny prostředků nebo předplatného](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Upozorňujeme, že pokud chcete upgradovat předplatné Azure, například přejít z bezplatného předplatného na placené, budete muset předplatné převést.

- Pokud chcete upgradovat bezplatnou zkušební verzi, podívejte se na článek Upgrade bezplatné zkušební verze nebo [předplatné Microsoft Imagine Azure na Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Informace o změně účtu placených služeb najdete v tématu Změna předplatného [Azure Pay-As-You-Go na jinou nabídku](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Přidání nebo přidružení předplatného Azure ke svému Azure Active Directory tenantovi:**

1. Přihlaste se a vyberte předplatné, které chcete použít, na stránce [Předplatná na portálu Azure Portal.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Vyberte **Změnit adresář**.
3. Zkontrolujte upozornění, která se zobrazí, a pak vyberte **Změnit**.
4. Adresář se u předplatného změní a zobrazí se zpráva o úspěchu.
5. K *přechodu* do nového adresáře použijte přepínač Adresář. Může to trvat až 10 minut, než se všechno správně zobrazí.

**Doporučené dokumenty**

- [Převedení vlastnictví předplatného Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Přesunutí zdrojů do nové skupiny prostředků nebo předplatného](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Správa prostředků pomocí portálu Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
