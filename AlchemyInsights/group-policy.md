---
title: Zásady skupiny
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256681"
---
# <a name="group-policy"></a><span data-ttu-id="b1cc5-102">Zásady skupiny</span><span class="sxs-lookup"><span data-stu-id="b1cc5-102">Group policy</span></span>

<span data-ttu-id="b1cc5-103">Nastavení pro objekty uživatelů a počítačů v Azure služba Active Directory Domain Services (Azure služba AD DS) se často spravují pomocí Zásady skupiny objektů (GPOs).</span><span class="sxs-lookup"><span data-stu-id="b1cc5-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="b1cc5-104">Azure služba AD DS obsahuje integrované gpOs pro uživatele AADDC a kontejnery AADDC Computers.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="b1cc5-105">Tyto předdefinové gpOs můžete přizpůsobit a konfigurovat zásady skupiny podle potřeby ve vašem prostředí.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="b1cc5-106">Členové skupiny správců Azure AD DC mají oprávnění pro správu zásad skupiny v doméně Azure služba AD DS a můžou taky vytvářet vlastní GPO a organizační jednotky.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="b1cc5-107">Další informace o zásadách skupiny a o tom, jak fungují, najdete [v Zásady skupiny přehledu.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="b1cc5-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="b1cc5-108">V hybridním prostředí se zásady skupiny nakonfigurované v místním služba AD DS nesynchronují s Azure služba AD DS.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="b1cc5-109">Pokud chcete definovat nastavení konfigurace pro uživatele nebo počítače v Azure služba AD DS, upravte jednu z výchozích zásad skupiny zásad skupiny nebo vytvořte vlastní objekt zásad skupiny.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="b1cc5-110">V tomto [článku se Zásady skupiny,](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) jak nainstalovat nástroje pro správu Zásady skupiny, jak upravit integrované gpOs a jak vytvářet vlastní GPO.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



