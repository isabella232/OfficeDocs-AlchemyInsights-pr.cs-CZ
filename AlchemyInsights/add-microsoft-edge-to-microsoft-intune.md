---
title: Přidání aplikace Microsoft Edge do Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194461"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="18a52-102">Přidání aplikace Microsoft Edge do Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="18a52-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="18a52-103">Abyste mohli nasadit, nakonfigurovat, monitorovat a chránit Microsoft Edge pro Windows 10, musíte ho nejdřív přidat do Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="18a52-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="18a52-104">Intune podporuje Microsoft Edge 77 a novější verze.</span><span class="sxs-lookup"><span data-stu-id="18a52-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="18a52-105">Intune rozpozná všechny už existující instalace Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="18a52-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="18a52-106">Pokud je Microsoft Edge nainstalovaný v kontextu uživatele, instalace systému přepíše instalaci v kontextu uživatele.</span><span class="sxs-lookup"><span data-stu-id="18a52-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="18a52-107">Pokud je Microsoft Edge nainstalovaný v kontextu systému, zobrazí se hlášení o úspěšné instalaci.</span><span class="sxs-lookup"><span data-stu-id="18a52-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="18a52-108">Předinstalovaný Microsoft Edge 77 a novější verze se pro všechny kanály v uživatelském kontextu přepíší s nainstalovanou aplikací Microsoft Edge v kontextu systému.</span><span class="sxs-lookup"><span data-stu-id="18a52-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="18a52-109">**Předpoklady**</span><span class="sxs-lookup"><span data-stu-id="18a52-109">**Prerequisite**</span></span>

<span data-ttu-id="18a52-110">Windows 10 verze 1709 nebo novější verze</span><span class="sxs-lookup"><span data-stu-id="18a52-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="18a52-111">**Postup přidání Edge do Intune**</span><span class="sxs-lookup"><span data-stu-id="18a52-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="18a52-112">[Nakonfigurujte aplikaci v Intune.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="18a52-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="18a52-113">[Nakonfigurujte informace o aplikaci.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="18a52-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="18a52-114">[Nakonfigurujte nastavení aplikace.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="18a52-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="18a52-115">[Vyberte značky oboru (volitelné).](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="18a52-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="18a52-116">[Přidejte aplikaci.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="18a52-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="18a52-117">Další nápovědu najdete v tématu [Řešení potíží.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="18a52-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




