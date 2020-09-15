---
title: Poradce při potížích s odepřením přístupu na weby OneDrivu pro firmy
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670609"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="efc09-102">Poradce při potížích s odepřením přístupu na weby OneDrivu pro firmy</span><span class="sxs-lookup"><span data-stu-id="efc09-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="efc09-103">K tomuto problému dochází často, když se uživatel odstraní a znovu vytvoří se stejným hlavním názvem uživatele (UPN).</span><span class="sxs-lookup"><span data-stu-id="efc09-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="efc09-104">Nový účet je vytvořen pomocí jiného identifikátoru PUID (kód účtu služby Passport).</span><span class="sxs-lookup"><span data-stu-id="efc09-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="efc09-105">Když se uživatel pokusí získat přístup ke kolekci webů nebo k OneDrivu, má nesprávný PUID.</span><span class="sxs-lookup"><span data-stu-id="efc09-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="efc09-106">Druhý scénář zahrnuje synchronizaci adresářů s organizační jednotkou služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="efc09-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="efc09-107">Pokud se uživatelé už přihlásili k SharePointu a pak jsou přesunuti na jinou organizační jednotku a znovu se synchronizují se SharePointem, může dojít k těmto potížím.</span><span class="sxs-lookup"><span data-stu-id="efc09-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="efc09-108">Tento problém vyřešíte tak, že obnovíte původní název UPN pomocí kroků v článku [obnovení uživatele v Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="efc09-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="efc09-109">Pokud původního uživatele obnovit nemůžete, odeberte ho z webu OneDrivu tímto postupem tak, že [odeberete uživatele ze seznamu informace o uživateli]().</span><span class="sxs-lookup"><span data-stu-id="efc09-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="efc09-110">Po dokončení této akce můžete ověřit, jestli má uživatel práva správce na web OneDrivu podle pokynů pro [Přidání správce na OneDrivu pro uživatele](https://docs.microsoft.com/sharepoint/manage-user-profiles) .</span><span class="sxs-lookup"><span data-stu-id="efc09-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="efc09-111">Další informace o úrovních oprávnění najdete v článku [Principy úrovní oprávnění v SharePointu](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="efc09-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
