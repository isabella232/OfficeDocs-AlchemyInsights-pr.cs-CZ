---
title: Přidání skupiny na web služby SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771192"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="1a83e-102">Problémy při vytváření skupinového propojeného webu na SharePointu</span><span class="sxs-lookup"><span data-stu-id="1a83e-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="1a83e-103">Vyskytly se některé běžné problémy při vytváření nebo opětovném vytváření skupinového propojeného webu.</span><span class="sxs-lookup"><span data-stu-id="1a83e-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="1a83e-104">Pokud jste odstranili skupinu a její připojený web a chcete vytvořit další web se stejnou adresou URL, budete muset trvale odebrat předchozí Web.</span><span class="sxs-lookup"><span data-stu-id="1a83e-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="1a83e-105">Stáhnout [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="1a83e-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="1a83e-106">Další informace o úvodním prostředí PowerShellu najdete v tématu [Začínáme se službou SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="1a83e-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="1a83e-107">Odeberte web z odstraněných webů pomocí rutiny [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1a83e-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="1a83e-108">K trvalému odstranění skupinových webů je potřeba PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1a83e-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="1a83e-109">Pokud vytváříte web připojený ke skupině a dostanete upozornění: **už existuje jiná skupina se stejným aliasem**, podívejte se na existující skupiny v centru pro [správu Microsoftu 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="1a83e-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="1a83e-110">Tento problém vyřešíte tak, že odstraníte existující skupinu, pokud ji už nepotřebujete nebo pokud chcete vytvořit web s jiným přiřazeným aliasem.</span><span class="sxs-lookup"><span data-stu-id="1a83e-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="1a83e-111">Moderní skupiny se SharePointem můžete vytvářet a používat různými způsoby.</span><span class="sxs-lookup"><span data-stu-id="1a83e-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="1a83e-112">Existující weby můžete připojit ke skupině Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1a83e-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="1a83e-113">Další informace najdete v článku [připojení skupiny Microsoft 365 pomocí uživatelského rozhraní SharePointu](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="1a83e-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="1a83e-114">Pokud chcete vytvořit web s připojenou skupinou Microsoft 365, budete muset vytvořit [týmový web](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="1a83e-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
