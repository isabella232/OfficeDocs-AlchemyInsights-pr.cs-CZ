---
title: 646 jak nakonfigurovat AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704482"
---
# <a name="configure-sync-features"></a><span data-ttu-id="aa74f-102">Konfigurace funkcí synchronizace</span><span class="sxs-lookup"><span data-stu-id="aa74f-102">Configure sync features</span></span>

<span data-ttu-id="aa74f-103">Azure AD Connect obsahuje několik funkcí, které jsou ve výchozím nastavení povolené, nebo je můžete povolit později.</span><span class="sxs-lookup"><span data-stu-id="aa74f-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="aa74f-104">Některé funkce vyžadují další konfiguraci v konkrétních prostředích.</span><span class="sxs-lookup"><span data-stu-id="aa74f-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="aa74f-105">[Filtrování](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) omezení: objekty jsou synchronizovány do služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="aa74f-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="aa74f-106">Ve výchozím nastavení se synchronizují všichni uživatelé, kontakty, skupiny a účty počítačů s Windows 10.</span><span class="sxs-lookup"><span data-stu-id="aa74f-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="aa74f-107">Můžete zahrnout nebo vyloučit objekty na základě domén, organizačních jednotek nebo jiných atributů.</span><span class="sxs-lookup"><span data-stu-id="aa74f-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="aa74f-108">[Synchronizace hash hesla](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) : synchronizuje hodnotu hash hesla z místní služby Active Directory do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="aa74f-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="aa74f-109">To umožňuje správu hesel v jednom umístění, ale používat stejné heslo v místním i cloudovém prostředí.</span><span class="sxs-lookup"><span data-stu-id="aa74f-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="aa74f-110">Protože je služba Active Directory autoritativním zdrojem, můžete použít vlastní zásady hesel.</span><span class="sxs-lookup"><span data-stu-id="aa74f-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="aa74f-111">[Samoobslužné resetování hesla (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umožňuje uživatelům resetovat si svoje vlastní hesla v cloudu i při používání místních zásad hesel.</span><span class="sxs-lookup"><span data-stu-id="aa74f-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="aa74f-112">[Zpětný zápis zařízení](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umožňuje, aby registrovaná zařízení v Azure AD byla zapsána zpátky do místní služby Active Directory, aby se mohla používat pro podmíněný přístup.</span><span class="sxs-lookup"><span data-stu-id="aa74f-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="aa74f-113">Možnost [zabránit nechtěným odstraněním](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je ve výchozím nastavení zapnutá, aby se zabránilo přílišnému počtu současných odstranění objektů (více než 500 objektů na synchronizaci).</span><span class="sxs-lookup"><span data-stu-id="aa74f-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="aa74f-114">Toto nastavení můžete změnit podle potřeb vaší organizace.</span><span class="sxs-lookup"><span data-stu-id="aa74f-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="aa74f-115">[Automatický upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je ve výchozím nastavení povolený pro Expresní instalace a pomáhá zajistit, že vaše verze Azure AD Connect je vždycky aktuální.</span><span class="sxs-lookup"><span data-stu-id="aa74f-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
