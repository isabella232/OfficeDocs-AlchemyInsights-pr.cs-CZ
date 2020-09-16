---
title: Poradce při potížích s odepřením přístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767651"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="3fb17-102">Řešení potíží s odepřením přístupu v centru pro správu SharePointu/OneDrivu</span><span class="sxs-lookup"><span data-stu-id="3fb17-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="3fb17-103">Pokud se při pokusu o přechod do centra pro správu SharePointu a OneDrivu zobrazuje zpráva o odepření přístupu, ujistěte se, že [uživateli přiřadíte licenci](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="3fb17-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="3fb17-104">Pokud má uživatel licenci, měli byste také ověřit, že je jim [přiřazena role správce](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , která má přístup k centrům pro správu.</span><span class="sxs-lookup"><span data-stu-id="3fb17-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="3fb17-105">Tento problém může také nastat, když se uživatel odstraní a znovu vytvoří se stejným hlavním názvem uživatele (UPN).</span><span class="sxs-lookup"><span data-stu-id="3fb17-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="3fb17-106">Nový účet je vytvořen pomocí jiného identifikátoru PUID (kód účtu služby Passport).</span><span class="sxs-lookup"><span data-stu-id="3fb17-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="3fb17-107">Když se uživatel pokusí získat přístup ke kolekci webů nebo k OneDrivu, má nesprávný PUID.</span><span class="sxs-lookup"><span data-stu-id="3fb17-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="3fb17-108">Druhý scénář zahrnuje synchronizaci adresářů s organizační jednotkou služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3fb17-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="3fb17-109">Pokud se uživatelé už přihlásili k SharePointu a pak jsou přesunuti na jinou organizační jednotku a znovu se synchronizují se SharePointem, může dojít k těmto potížím.</span><span class="sxs-lookup"><span data-stu-id="3fb17-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="3fb17-110">Tento problém vyřešíte tak, že obnovíte původní uživatelské jméno (UPN) pomocí kroků v tomto článku a [obnovíte uživatele v Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="3fb17-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="3fb17-111">Poznámka: Pokud centrum pro správu OneDrivu nebo SharePointu není dostupné pro víc uživatelů, kteří mají přístup dřív, může se jednat o dočasný problém služby.</span><span class="sxs-lookup"><span data-stu-id="3fb17-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="3fb17-112">[Zkontrolujte řídicí panel stavu služeb](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="3fb17-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


