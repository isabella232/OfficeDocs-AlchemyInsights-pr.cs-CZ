---
title: Synchronizace hodnot hash hesel u služby domény
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177383"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="0402f-102">Synchronizace hodnot hash hesel u služby domény</span><span class="sxs-lookup"><span data-stu-id="0402f-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="0402f-103">**Pokud instance Azure služba AD DS vás vyzve k povolení synchronizace hodnot hash hesel**</span><span class="sxs-lookup"><span data-stu-id="0402f-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="0402f-104">Narazíte na scénář, ve kterém používáte hybridní prostředí s uživateli, kteří se synchronizují z místního prostředí Azure služba Active Directory Domain Services (služba AD DS).</span><span class="sxs-lookup"><span data-stu-id="0402f-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="0402f-105">Tento scénář se setkávají i přes to, že máte synchronizaci hodnot hash hesel z místní služba AD DS do vašeho tenanta Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0402f-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="0402f-106">Tato část obsahuje přehledné informace o problému a osobě, která ho má odstranit. Na obrázku vidíte tři základní strany v transakci e-mailu Office 365 - odesílatele, Office 365 a příjemce. Červeně označená oblast je oblast, ve které je obvykle potřeba problém odstranit.</span><span class="sxs-lookup"><span data-stu-id="0402f-106">**Cause**</span></span>

<span data-ttu-id="0402f-107">K tomu dochází proto, že Azure AD Connect ve výchozím nastavení nesynchronuje starší hodnoty hash hesel NTLM (New Technology LAN Manager) a Kerberos, které jsou potřeba pro Azure služba AD DS.</span><span class="sxs-lookup"><span data-stu-id="0402f-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="0402f-108">**Řešení**</span><span class="sxs-lookup"><span data-stu-id="0402f-108">**Workaround**</span></span> 

<span data-ttu-id="0402f-109">Aby bylo možné synchronizovat tyto a hash hesel požadované pro ověřování NTLM a Kerberos, bude potřeba nakonfigurovat Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="0402f-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="0402f-110">Po nakonfigurování Azure AD Connect pak místní událost pro vytvoření účtu nebo změnu hesla také synchronizuje starší hash hesel do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0402f-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="0402f-111">V tomto [článku najdete](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) další informace a pokyny k povolení synchronizace hesel v hybridním prostředí Azure služba AD DS Azure.</span><span class="sxs-lookup"><span data-stu-id="0402f-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>