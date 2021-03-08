---
title: Protokoly hesel
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50524118"
---
# <a name="password-logs"></a><span data-ttu-id="6846c-102">Protokoly hesel</span><span class="sxs-lookup"><span data-stu-id="6846c-102">Password logs</span></span>

<span data-ttu-id="6846c-103">**Mám problémy s přístupem k protokolům auditování při resetování hesla**</span><span class="sxs-lookup"><span data-stu-id="6846c-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="6846c-104">Pokud chcete vyřešit problémy s přístupem k protokolům auditování resetování hesla, proveďte následující krok:</span><span class="sxs-lookup"><span data-stu-id="6846c-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="6846c-105">Ujistěte se, že máte oprávnění k zobrazení protokolů auditování.</span><span class="sxs-lookup"><span data-stu-id="6846c-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="6846c-106">Autorizované jsou jenom tyto role:</span><span class="sxs-lookup"><span data-stu-id="6846c-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="6846c-107">Globální správce</span><span class="sxs-lookup"><span data-stu-id="6846c-107">Global administrator</span></span>
 - <span data-ttu-id="6846c-108">Správce zabezpečení</span><span class="sxs-lookup"><span data-stu-id="6846c-108">Security administrator</span></span>
 - <span data-ttu-id="6846c-109">Čtenář zabezpečení</span><span class="sxs-lookup"><span data-stu-id="6846c-109">Security reader</span></span>

<span data-ttu-id="6846c-110">**Chci zobrazit všechny události auditování resetování hesel od okamžiku, kdy jsem ho poprvé nasazoval(a).**</span><span class="sxs-lookup"><span data-stu-id="6846c-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="6846c-111">V sestavách za posledních 30 dní se uloží až 120 000 událostí pro resetování/registraci hesel.</span><span class="sxs-lookup"><span data-stu-id="6846c-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="6846c-112">Tento maximální limit platí pro uživatelské rozhraní při stahování souboru CSV.</span><span class="sxs-lookup"><span data-stu-id="6846c-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="6846c-113">Přes PowerShell je dostupný 1 milion událostí.</span><span class="sxs-lookup"><span data-stu-id="6846c-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="6846c-114">Další informace najdete pod následujícími odkazy:</span><span class="sxs-lookup"><span data-stu-id="6846c-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="6846c-115">Události samoobslužného resetování hesla z rozhraní API sestav a událostí Azure AD</span><span class="sxs-lookup"><span data-stu-id="6846c-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="6846c-116">Jak rychle stáhnout události registrace resetování hesla pomocí PowerShellu</span><span class="sxs-lookup"><span data-stu-id="6846c-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="6846c-117">**Chci se dozvědět víc o možnostech vytváření sestav pro resetování hesel**</span><span class="sxs-lookup"><span data-stu-id="6846c-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="6846c-118">Zkontrolujte, kdo registruje nebo resetuje hesla pomocí protokolů auditování hesel Azure AD na portálu Azure Portal v části Uživatelé a **skupiny.**</span><span class="sxs-lookup"><span data-stu-id="6846c-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="6846c-119">Další informace najdete na těchto odkazech:</span><span class="sxs-lookup"><span data-stu-id="6846c-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="6846c-120">Přehled sestav resetování hesla</span><span class="sxs-lookup"><span data-stu-id="6846c-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="6846c-121">Jak zobrazit sestavy pro resetování hesla na portálu Azure Portal</span><span class="sxs-lookup"><span data-stu-id="6846c-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="6846c-122">Události samoobslužného resetování hesla z rozhraní API sestav a událostí Azure AD</span><span class="sxs-lookup"><span data-stu-id="6846c-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="6846c-123">Jak rychle stáhnout události registrace resetování hesla pomocí PowerShellu</span><span class="sxs-lookup"><span data-stu-id="6846c-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


