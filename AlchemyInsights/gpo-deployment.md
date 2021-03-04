---
title: Nasazení objektu zásad skupiny
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427087"
---
# <a name="gpo-deployment"></a><span data-ttu-id="6c3fe-102">Nasazení objektu zásad skupiny</span><span class="sxs-lookup"><span data-stu-id="6c3fe-102">GPO Deployment</span></span>

<span data-ttu-id="6c3fe-103">Nastavení pro objekty uživatelů a počítačů v Azure služba Active Directory Domain Services (Azure služba AD DS) se často spravují pomocí Zásady skupiny objektů (GPOs).</span><span class="sxs-lookup"><span data-stu-id="6c3fe-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="6c3fe-104">Azure služba AD DS obsahuje integrované gpOs pro uživatele AADDC a kontejnery AADDC Computers.</span><span class="sxs-lookup"><span data-stu-id="6c3fe-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="6c3fe-105">Tyto předdefinové gpOs můžete přizpůsobit a konfigurovat zásady skupiny podle potřeby ve vašem prostředí.</span><span class="sxs-lookup"><span data-stu-id="6c3fe-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="6c3fe-106">Členové skupiny správců Azure AD DC mají oprávnění pro správu zásad skupiny v doméně Azure služba AD DS a můžou taky vytvářet vlastní GPO a organizační jednotky.</span><span class="sxs-lookup"><span data-stu-id="6c3fe-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="6c3fe-107">Další informace o zásadách skupiny a o tom, jak fungují, najdete v [Zásady skupiny přehledu.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="6c3fe-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="6c3fe-108">V hybridním prostředí se zásady skupiny nakonfigurované v místním služba AD DS nesynchronují s Azure služba AD DS.</span><span class="sxs-lookup"><span data-stu-id="6c3fe-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="6c3fe-109">Pokud chcete definovat nastavení konfigurace pro uživatele nebo počítače v Azure služba AD DS, upravte jednu z výchozích zásad skupiny zásad skupiny nebo vytvořte vlastní objekt zásad skupiny.</span><span class="sxs-lookup"><span data-stu-id="6c3fe-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="6c3fe-110">V tomto [článku se Zásady skupiny,](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) jak nainstalovat nástroje pro správu Zásady skupiny, jak upravit integrované gpOs a jak vytvářet vlastní GPO.</span><span class="sxs-lookup"><span data-stu-id="6c3fe-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
