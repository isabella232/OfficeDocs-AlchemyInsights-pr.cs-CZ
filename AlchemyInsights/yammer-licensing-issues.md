---
title: Problémy s licencováním Yammeru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148200"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="07b8b-102">Problémy s licencováním Yammeru</span><span class="sxs-lookup"><span data-stu-id="07b8b-102">Yammer licensing issues</span></span>

<span data-ttu-id="07b8b-103">Všichni uživatelé musí mít licenci k používání služby Yammer Enterprise, ale ve výchozím nastavení Yammer nevyžaduje, aby uživatelé měli licenci pro přístup ke službě.</span><span class="sxs-lookup"><span data-stu-id="07b8b-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="07b8b-104">Když správce změní nastavení tak, aby blokoval uživatele Microsoft 365 bez licencí Yammeru, uživatelé, kterým není přiřazena licence Yammeru Enterprise, nemají přístup ke službě Yammer.</span><span class="sxs-lookup"><span data-stu-id="07b8b-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="07b8b-105">Další informace najdete [v tématu Správa uživatelských licencí Yammeru v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="07b8b-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="07b8b-106">Když jsou licence odebrány uživatelům, dlaždice Yammeru se už nezobrazí a ostatní služby můžou pomocí odebrání licence skrýt funkce.</span><span class="sxs-lookup"><span data-stu-id="07b8b-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="07b8b-107">V ostatních případech se funkce mohou stále zobrazovat, ale vyžadují přiřazení licence k provozu.</span><span class="sxs-lookup"><span data-stu-id="07b8b-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="07b8b-108">**Licence se pro uživatele neaktualizuje.**</span><span class="sxs-lookup"><span data-stu-id="07b8b-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="07b8b-109">V některých příležitostech je uživateli přiřazena licence, ale stále nemůže získat přístup k Yammeru.</span><span class="sxs-lookup"><span data-stu-id="07b8b-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="07b8b-110">Zpoždění je pravděpodobnější, když probíhá hromadné přiřazení licence.</span><span class="sxs-lookup"><span data-stu-id="07b8b-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="07b8b-111">Uživatelé Yammeru nemusí být aktualizováni ve stejném pořadí, jako licence se mění ve službě Azure AD, protože systém běží asynchronně.</span><span class="sxs-lookup"><span data-stu-id="07b8b-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="07b8b-112">Před otevřením případu podpory počkejte až 24 hodin a nahlaste problémy se synchronizací licencí.</span><span class="sxs-lookup"><span data-stu-id="07b8b-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="07b8b-113">**Hromadné přiřazení licence**</span><span class="sxs-lookup"><span data-stu-id="07b8b-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="07b8b-114">Licence lze přiřadit prostřednictvím centra pro správu nebo skriptování prostředí PowerShell.</span><span class="sxs-lookup"><span data-stu-id="07b8b-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="07b8b-115">Další informace najdete v tématech [Přiřazení licencí uživatelům](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) a Přiřazení licencí [uživatelským účtům pomocí Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="07b8b-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="07b8b-116">Podpora společnosti Microsoft neposkytuje pomoc při vytváření skriptů, ale je k dispozici dokumentace k přiřazení licencí Yammeru.</span><span class="sxs-lookup"><span data-stu-id="07b8b-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="07b8b-117">Další informace najdete v [tématu Správa licencí Yammeru pomocí prostředí Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="07b8b-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>