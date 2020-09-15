---
title: Kód chyby 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Pokud se při aktivaci Office 2013 na nasazení služby Vzdálená plocha (RDS) zobrazuje chyba, zvažte povolení funkce ADAL úpravou registru.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709180"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="2c9d9-103">Chyba při aktivaci Office 2013 na vzdálené ploše</span><span class="sxs-lookup"><span data-stu-id="2c9d9-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="2c9d9-104">Pokud se při aktivaci Office 2013 na nasazení služby Vzdálená plocha (RDS) zobrazuje chyba, zvažte povolení funkce ADAL úpravou registru.</span><span class="sxs-lookup"><span data-stu-id="2c9d9-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="2c9d9-105">**Klíč registru**</span><span class="sxs-lookup"><span data-stu-id="2c9d9-105">**Registry key**</span></span>|<span data-ttu-id="2c9d9-106">**Typ**</span><span class="sxs-lookup"><span data-stu-id="2c9d9-106">**Type**</span></span>|<span data-ttu-id="2c9d9-107">**Hodnota**</span><span class="sxs-lookup"><span data-stu-id="2c9d9-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2c9d9-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="2c9d9-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="2c9d9-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="2c9d9-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="2c9d9-110">0,1</span><span class="sxs-lookup"><span data-stu-id="2c9d9-110">1</span></span>  <br/> |

<span data-ttu-id="2c9d9-111">Další informace najdete v tématu [Povolení moderního ověřování pro Office 2013 na zařízeních s Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="2c9d9-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="2c9d9-112">ADAL je ve výchozím nastavení aplikací Microsoft 365 pro podniky a Office 2016 povolen.</span><span class="sxs-lookup"><span data-stu-id="2c9d9-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="2c9d9-113">Vzdálená plocha (RDS) se dřív jmenovala Terminálová služba.</span><span class="sxs-lookup"><span data-stu-id="2c9d9-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  