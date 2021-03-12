---
title: Poradce při potížích se zprávami s odepření přístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707947"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="5fc9e-102">Poradce při potížích se zprávami o odepření přístupu v Centru pro správu SharePointu nebo OneDrivu</span><span class="sxs-lookup"><span data-stu-id="5fc9e-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="5fc9e-103">Pokud se vám při pokusu o procházení do Centra pro správu SharePointu nebo OneDrivu zobrazí zpráva o odepření přístupu, ujistěte se, že jste uživateli [přiřadili licenci.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="5fc9e-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="5fc9e-104">Pokud má uživatel licenci, měli byste se ujistit, že má přiřazenou [roli](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) správce, která má přístup k centrem pro správu.</span><span class="sxs-lookup"><span data-stu-id="5fc9e-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="5fc9e-105">K tomuto problému může také dojít, když se uživatel odstraní a znovu vytvoří se stejným hlavním názvem uživatele (UPN).</span><span class="sxs-lookup"><span data-stu-id="5fc9e-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="5fc9e-106">Nový účet se vytvoří pomocí jiné hodnoty ID uživatelského účtu (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="5fc9e-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="5fc9e-107">Když se uživatel pokusí o přístup ke kolekci webů nebo k jejich OneDrivu, má uživatel nesprávný KÓD PUID.</span><span class="sxs-lookup"><span data-stu-id="5fc9e-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="5fc9e-108">Druhý scénář zahrnuje synchronizaci adresářů s organizační jednotkou služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5fc9e-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="5fc9e-109">Pokud se už uživatelé přihlásili k SharePointu a pak se přesunou do jiné OU a budou se znovu synchronizovat se SharePointem, mohou zaznamenat tento problém.</span><span class="sxs-lookup"><span data-stu-id="5fc9e-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="5fc9e-110">Tento problém vyřešíte tak, že obnovíte původní hlavní název uživatele pomocí postupu v článku Obnovení [uživatele v Microsoftu 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="5fc9e-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="5fc9e-111">Poznámka: Pokud není Centrum pro správu OneDrivu nebo SharePointu dostupné více uživatelům, kteří k přístupu měli předtím přístup, může jít o dočasný problém se službou.</span><span class="sxs-lookup"><span data-stu-id="5fc9e-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="5fc9e-112">[Zkontrolujte řídicí panel stavu služby.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="5fc9e-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


