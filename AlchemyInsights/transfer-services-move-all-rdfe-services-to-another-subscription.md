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
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691977"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Přenos služeb – přesunutí všech služeb RDFE do jiného předplatného

**Přesunutí zdrojů**

Prostředky Azure se dají přesunout do jiného předplatného Azure nebo skupiny prostředků pod stejným předplatným pomocí Azure Portal, Azure PowerShellu, Azure CLI nebo REST API pro přesouvání prostředků.

Než budete moct přesunout zdroje, přečtěte si téma:

- [Kontrolní seznam před přesunutím zdrojů](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Služby, které lze přesunout](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Jak ověřit přesunutí](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Přesunutí pokynů pro služby](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Pokud chcete přesunout existující zdroje do jiné skupiny zdrojů nebo předplatného, můžete použít:

- [Portál Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Kurz: [přesunutí zdrojů Azure do jiné skupiny zdrojů nebo předplatného](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Poradce při potížích se správcem prostředků Azure**

Informace o některých běžných chybách nasazení Azure a získávání informací pro jejich řešení najdete v článcích níže. Pokud kód chyby chyby nasazení nemůžete najít, přečtěte si téma [vyhledání kódu chyby](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Řešení chyb nasazení](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Řešení potíží při přesouvání prostředků Azure do nové skupiny zdrojů nebo předplatného](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Uvědomte si, že pokud si přejete upgradovat předplatné Azure, třeba přepnout z bezplatného na to-to-do, budete muset předplatné převést.

- Pokud chcete upgradovat bezplatnou zkušební verzi, přečtěte si článek [upgrade bezplatného zkušebního předplatného společnosti Microsoft](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)a vyzkoušejte si předplatné Azure.
- Pokud chcete změnit účet s účtem s účtem, přečtěte si článek [Změna předplatného služby Azure Pay-as-to-go na jinou nápovědu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Přidání nebo přidružení předplatného Azure ke svému tenantovi Azure Active Directory:**

1. Přihlaste se a vyberte předplatné, které chcete použít na [stránce Předplatná na portálu Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Vyberte **změnit adresář**.
3. Zkontrolujte všechna zobrazená upozornění a pak vyberte **změnit**.
4. U předplatného se změní adresář a zobrazí se zpráva o úspěšném dokončení.
5. Pomocí přepínače *adresáře* přejděte do nového adresáře. Zobrazení obsahu může trvat až 10 minut.

**Doporučené dokumenty**

- [Převod vlastnictví předplatného Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Přesunutí zdrojů do nové skupiny zdrojů nebo do nového předplatného](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Správa zdrojů pomocí Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
