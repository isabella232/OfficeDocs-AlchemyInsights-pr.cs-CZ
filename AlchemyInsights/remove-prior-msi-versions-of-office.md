---
title: Odebrání předchozích verzí Office MSI
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680659"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="e5ba7-102">Odebrání předchozích verzí Office MSI</span><span class="sxs-lookup"><span data-stu-id="e5ba7-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="e5ba7-103">Doporučuje se před instalací Office 365 proplusm odebrat starší verze Office pro instalační službu systému Windows (MSI).</span><span class="sxs-lookup"><span data-stu-id="e5ba7-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="e5ba7-104">Tady je postup:</span><span class="sxs-lookup"><span data-stu-id="e5ba7-104">Here's how to do this:</span></span>

1. <span data-ttu-id="e5ba7-105">Pokud jste k instalaci Office použili instalační program MSI, můžete Office odinstalovat pomocí nástroje pro nasazení Office.</span><span class="sxs-lookup"><span data-stu-id="e5ba7-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="e5ba7-106">V souboru **configuration.xml** můžete použít prvek RemoveMSI.</span><span class="sxs-lookup"><span data-stu-id="e5ba7-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="e5ba7-107">Postupujte podle pokynů v tomto článku: [Centrum zabezpečení Office 365 Security &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="e5ba7-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>