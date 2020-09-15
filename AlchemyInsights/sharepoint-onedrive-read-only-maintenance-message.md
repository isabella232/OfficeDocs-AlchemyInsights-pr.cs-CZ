---
title: Zpráva o údržbě určená jen pro čtení při pokusu o použití SharePointu nebo OneDrivu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670825"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="977a3-102">Zpráva o údržbě určená jen pro čtení při pokusu o použití SharePointu nebo OneDrivu</span><span class="sxs-lookup"><span data-stu-id="977a3-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="977a3-103">Při pokusu o použití SharePointu nebo OneDrivu pro některý z následujících scénářů se uživatelům může zobrazit zpráva o **údržbě jen pro čtení** .</span><span class="sxs-lookup"><span data-stu-id="977a3-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="977a3-104">Plánovaná nebo aktivní aktivita údržby.</span><span class="sxs-lookup"><span data-stu-id="977a3-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="977a3-105">Podívejte se na ně tak, že přejdete do [centra zpráv](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="977a3-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="977a3-106">S vysokou prioritou aktivní servisní události, ke které může dojít.</span><span class="sxs-lookup"><span data-stu-id="977a3-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="977a3-107">Podívejte se na všechny informační zpravodaje/incidenty – přejděte na [stav služby](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="977a3-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="977a3-108">Nepatrný automatický způsob obnovení, který může nastat kvůli neočekávaným událostem na serverech, které by mohly trvat méně než 30 min.</span><span class="sxs-lookup"><span data-stu-id="977a3-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="977a3-109">U těchto menších obnovení nejsou k dispozici žádná centra zpráv nebo služby stavu služeb, ale měli byste být zpátky na normální.</span><span class="sxs-lookup"><span data-stu-id="977a3-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="977a3-110">Na krátkou chvíli jsme narazili na to, že jedna ze tří uvedených scénářů byla příčina, a služba byla obnovena, ale mezipaměť prohlížeče uživatelů nebyla smazána.</span><span class="sxs-lookup"><span data-stu-id="977a3-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="977a3-111">Než přejdete na web, zkuste vymazat mezipaměť prohlížeče.</span><span class="sxs-lookup"><span data-stu-id="977a3-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="977a3-112">V prohlížeči Microsoft Edge vyberte **Nastavení**a pak vyberte **Ochrana osobních údajů a zabezpečení**.</span><span class="sxs-lookup"><span data-stu-id="977a3-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="977a3-113">V části **Vymazat procházení**vyberte **zvolit, co chcete vymazat**.</span><span class="sxs-lookup"><span data-stu-id="977a3-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="977a3-114">Vyberte **soubory cookie a data uloženého webu**a vyberte **Vymazat**.</span><span class="sxs-lookup"><span data-stu-id="977a3-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="977a3-115">Tento postup se může lišit při používání jiných prohlížečů, jako je Mozilla Firefox nebo Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="977a3-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="977a3-116">Další možností je otevřít SharePointový web nebo OneDrive v novém okně InPrivate.</span><span class="sxs-lookup"><span data-stu-id="977a3-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>