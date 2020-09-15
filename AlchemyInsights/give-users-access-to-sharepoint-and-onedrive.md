---
title: Poskytnutí přístupu uživatelů k SharePointu a OneDrivu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677200"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="0f7d7-102">Poskytnutí přístupu uživatelů k SharePointu a OneDrivu</span><span class="sxs-lookup"><span data-stu-id="0f7d7-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="0f7d7-103">Pokud není SharePointový web dostupný pro víc uživatelů, kteří mají přístup dřív, může se jednat o dočasný problém služby.</span><span class="sxs-lookup"><span data-stu-id="0f7d7-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="0f7d7-104">Kontrola řídicího panelu stavu služeb</span><span class="sxs-lookup"><span data-stu-id="0f7d7-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="0f7d7-105">Pokud chcete, aby se lidé ve vaší organizaci mohli přihlásit a používat SharePoint a OneDrive, musíte pro ně přidat účty a zajistit, že mají licenci, která jim uděluje přístup k SharePointu a OneDrivu.</span><span class="sxs-lookup"><span data-stu-id="0f7d7-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="0f7d7-106">Nejjednodušším způsobem, jak přidat uživatele, je v centru pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0f7d7-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="0f7d7-107">Přejděte na [stránku aktivní uživatelé v centru pro správu Microsoft 365](https://portal.office.com/adminportal/home#/users)a klikněte na **Přidat uživatele**.</span><span class="sxs-lookup"><span data-stu-id="0f7d7-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="0f7d7-108">Vyplňte informace o uživateli a ujistěte se, že je v části **licence produktu**přiřazená licence a je vybrána **SharePoint Online** .</span><span class="sxs-lookup"><span data-stu-id="0f7d7-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="0f7d7-109">Pokud povolíte externí sdílení ve vaší organizaci, můžou uživatelé sdílet obsah SharePointu a OneDrivu s lidmi mimo organizaci.</span><span class="sxs-lookup"><span data-stu-id="0f7d7-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="0f7d7-110">Tyto externí uživatelské licence nemusíte poskytovat.</span><span class="sxs-lookup"><span data-stu-id="0f7d7-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="0f7d7-111">K těmto účtům nemusíte také přidávat účty, pokud není nastavené sdílení nastaveno na jenom stávající externí uživatele.</span><span class="sxs-lookup"><span data-stu-id="0f7d7-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="0f7d7-112">V takovém případě je třeba, aby uživatelé v adresáři vaší organizace byli přidáni jako uživatelé typu Host v centru pro správu služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0f7d7-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

