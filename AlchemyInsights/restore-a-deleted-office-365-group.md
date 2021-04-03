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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505679"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="03668-102">Obnovení odstraněné skupiny Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="03668-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="03668-103">Odstraněnou skupinu Microsoft 365 nebo Microsoft Teams můžete obnovit do 30 dnů od odstranění.</span><span class="sxs-lookup"><span data-stu-id="03668-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="03668-104">Pokud se chcete přihlásit do Centra pro správu Microsoftu 365 a zobrazit seznam odstraněných skupin a týmů, přejděte do Centra pro správu [Microsoftu 365.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="03668-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="03668-105">**Poznámka:** Přihlaste se pomocí účtu, který je přiřazený správci tenanta nebo roli správce skupin.</span><span class="sxs-lookup"><span data-stu-id="03668-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="03668-106">Vyberte odstraněnou skupinu Microsoft 365/Teams, která se má obnovit, a klikněte **na obnovit skupinu.**</span><span class="sxs-lookup"><span data-stu-id="03668-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="03668-107">Pokud skupinu nemůžete obnovit kvůli konfliktní adrese SMTP, použijte následující příkaz k vyhledání objektu, který způsobuje konflikt, a odeberte adresu SMTP:</span><span class="sxs-lookup"><span data-stu-id="03668-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="03668-108">**Poznámka:** V některých případech může trvat až 24 hodin, než se skupina a všechna její data obnoví.</span><span class="sxs-lookup"><span data-stu-id="03668-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="03668-109">Další informace nebo informace o obnovení skupin pomocí PowerShellu najdete v tématu Obnovení odstraněné skupiny [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="03668-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>