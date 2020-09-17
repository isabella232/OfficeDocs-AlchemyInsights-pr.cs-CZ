---
title: 932 upgrade AADConnect
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
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806032"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="ede7b-102">Upgrade služby Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="ede7b-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="ede7b-103">Ve výchozím nastavení je automatický upgrade povolený pro Azure AD Connect, který vám pomůže zajistit, že máte nejnovější verzi.</span><span class="sxs-lookup"><span data-stu-id="ede7b-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="ede7b-104">Pokud chcete ověřit nastavení automatického upgradu, použijte rutinu **Get-ADSyncAutoUpgrade** v Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ede7b-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="ede7b-105">Rutina vrátí jednu z následujících hodnot:</span><span class="sxs-lookup"><span data-stu-id="ede7b-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="ede7b-106">**Povoleno**: je povolen automatický upgrade.</span><span class="sxs-lookup"><span data-stu-id="ede7b-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="ede7b-107">**Zakázáno**: automatický upgrade je zakázán.</span><span class="sxs-lookup"><span data-stu-id="ede7b-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="ede7b-108">**Pozastaveno**: systém už neumožňuje přijímat automatické upgrady.</span><span class="sxs-lookup"><span data-stu-id="ede7b-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="ede7b-109">Tuto hodnotu nemůžete nakonfigurovat. je nastavená systémem.</span><span class="sxs-lookup"><span data-stu-id="ede7b-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="ede7b-110">Další informace najdete v tématu [Automatický upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="ede7b-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="ede7b-111">Pokud chcete stáhnout nejnovější verzi Azure AD Connect, přejděte na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="ede7b-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
