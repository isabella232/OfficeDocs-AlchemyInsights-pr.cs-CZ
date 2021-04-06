---
title: Obnovení odstraněné skupiny Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597436"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="cb921-102">Obnovení odstraněné skupiny Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="cb921-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="cb921-103">Odstraněnou skupinu Microsoft 365 nebo Microsoft Teams můžete obnovit do 30 dnů od odstranění.</span><span class="sxs-lookup"><span data-stu-id="cb921-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="cb921-104">Přejděte do [Centra pro správu Microsoftu 365 a](https://aka.ms/RestoreDeletedGroup) přihlaste se a seznam odstraněných skupin a týmů.</span><span class="sxs-lookup"><span data-stu-id="cb921-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in and list the deleted groups and teams.</span></span>

    <span data-ttu-id="cb921-105">**Poznámka:** Přihlaste se pomocí účtu, který je přiřazený správci tenanta nebo roli správce skupin.</span><span class="sxs-lookup"><span data-stu-id="cb921-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="cb921-106">Vyberte odstraněnou skupinu Microsoft 365/Teams, která se má obnovit, a klikněte **na obnovit skupinu.**</span><span class="sxs-lookup"><span data-stu-id="cb921-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="cb921-107">Pokud skupinu nemůžete obnovit kvůli konfliktní adrese SMTP, použijte následující příkaz k vyhledání objektu, který způsobuje konflikt, a odeberte adresu SMTP:</span><span class="sxs-lookup"><span data-stu-id="cb921-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="cb921-108">**Poznámka:** V některých případech může trvat až 24 hodin, než se skupina a všechna její data obnoví.</span><span class="sxs-lookup"><span data-stu-id="cb921-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="cb921-109">Další informace nebo informace o obnovení skupin pomocí PowerShellu najdete v tématu Obnovení odstraněné skupiny [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="cb921-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>