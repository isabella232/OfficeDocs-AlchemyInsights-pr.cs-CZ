---
title: V klientovi Microsoft Teams se nezobrazuje ikona kalendáře
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583345"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="fdc57-102">V klientovi Microsoft Teams se nezobrazuje ikona kalendáře</span><span class="sxs-lookup"><span data-stu-id="fdc57-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="fdc57-103">Karta **Kalendář** v aplikaci Teams vyžaduje přístup k poštovní schránce Exchange prostřednictvím webových služeb Exchange.</span><span class="sxs-lookup"><span data-stu-id="fdc57-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="fdc57-104">Poštovní schránka Exchange může být online nebo místní.</span><span class="sxs-lookup"><span data-stu-id="fdc57-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="fdc57-105">Uživatelům, kteří nevidí kartu **Kalendář** , se ujistěte, že [jsou licencovány pro poštovní schránku Exchange Online a že poštovní schránka je povolená](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="fdc57-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="fdc57-106">Pokud jsou vaši uživatelé místní, musíte potvrdit, že je vaše hybridní konfigurace v pořádku.</span><span class="sxs-lookup"><span data-stu-id="fdc57-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="fdc57-107">K řešení potíží použijte [průvodce hybridní konfigurací](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="fdc57-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="fdc57-108">Poznámka: [Teams vyžaduje Exchange 2016 CU3 nebo novější](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="fdc57-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="fdc57-109">Další informace a postupy řešení potíží najdete v článku [Poradce při potížích s interakcí Microsoft teams a Exchange serveru](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="fdc57-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
