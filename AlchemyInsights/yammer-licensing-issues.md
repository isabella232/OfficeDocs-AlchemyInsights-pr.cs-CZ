---
title: Problémy s licencováním Yammeru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657269"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="ef6cf-102">Problémy s licencováním Yammeru</span><span class="sxs-lookup"><span data-stu-id="ef6cf-102">Yammer licensing issues</span></span>

<span data-ttu-id="ef6cf-103">Všichni uživatelé musí mít licenci k používání služby Yammer Enterprise, ale ve výchozím nastavení Yammeru nevyžadují, aby uživatelé měli licenci pro přístup ke službě.</span><span class="sxs-lookup"><span data-stu-id="ef6cf-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="ef6cf-104">Když správce změní nastavení tak, aby blokoval uživatele Microsoft 365 bez licencí na Yammeru, uživatelé, kteří nemají přiřazenou licenci Yammeru Enterprise, nemají přístup ke službě Yammer.</span><span class="sxs-lookup"><span data-stu-id="ef6cf-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="ef6cf-105">Další informace najdete v tématu [Správa uživatelských licencí Yammeru v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) .</span><span class="sxs-lookup"><span data-stu-id="ef6cf-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="ef6cf-106">Po odebrání licencí uživatelům se dlaždice Yammeru už nezobrazuje a další služby můžou pomocí odebrání licence tyto funkce skrýt.</span><span class="sxs-lookup"><span data-stu-id="ef6cf-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="ef6cf-107">V ostatních případech se funkce mohou stále zobrazovat, ale vyžadují, aby fungovaly.</span><span class="sxs-lookup"><span data-stu-id="ef6cf-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="ef6cf-108">**Licence není pro uživatele aktualizovaná**</span><span class="sxs-lookup"><span data-stu-id="ef6cf-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="ef6cf-109">Uživateli je příležitostně přiřazena licence, ale stále neumožňuje přístup k Yammeru.</span><span class="sxs-lookup"><span data-stu-id="ef6cf-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="ef6cf-110">Prodleva se pravděpodobněji projeví při přiřazování hromadných licencí.</span><span class="sxs-lookup"><span data-stu-id="ef6cf-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="ef6cf-111">Uživatelé Yammeru se nemusí aktualizovat ve stejném pořadí, protože se v Azure AD změní licence, protože systém běží asynchronně.</span><span class="sxs-lookup"><span data-stu-id="ef6cf-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="ef6cf-112">Počkejte až 24 hodin před otevřením případu podpory k nahlášení problémů se synchronizací licencí.</span><span class="sxs-lookup"><span data-stu-id="ef6cf-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="ef6cf-113">**Hromadné přidělování licencí**</span><span class="sxs-lookup"><span data-stu-id="ef6cf-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="ef6cf-114">Licence se dají přiřadit prostřednictvím centra pro správu nebo skriptování PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="ef6cf-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="ef6cf-115">Další informace najdete v článku [přiřazení licencí uživatelům](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) a [přiřazení licencí uživatelským účtům pomocí Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="ef6cf-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="ef6cf-116">Podpora Microsoftu neposkytuje pomoc při vytváření skriptů, ale k dispozici je dokumentace k přiřazení licencí Yammeru.</span><span class="sxs-lookup"><span data-stu-id="ef6cf-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="ef6cf-117">Další informace najdete v tématu [Správa licencí Yammeru pomocí Windows PowerShellu](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="ef6cf-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>