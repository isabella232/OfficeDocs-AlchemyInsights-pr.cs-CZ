---
title: Oznámení AAD Connect
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035087"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="32e9c-102">Oznámení AAD Connect</span><span class="sxs-lookup"><span data-stu-id="32e9c-102">Notification AAD Connect</span></span>

- <span data-ttu-id="32e9c-103">Ujistěte se, že máte oprávnění k provedení operace.</span><span class="sxs-lookup"><span data-stu-id="32e9c-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="32e9c-104">Globální správci mají ve výchozím nastavení přístup.</span><span class="sxs-lookup"><span data-stu-id="32e9c-104">Global Admins have access by default.</span></span> <span data-ttu-id="32e9c-105">K delegování [](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) oprávnění k registraci přispěvateli můžete použít řízení přístupu založeného na rolích.</span><span class="sxs-lookup"><span data-stu-id="32e9c-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="32e9c-106">Zajistěte, aby byly povolené požadované koncové body a nebyly blokovány kvůli bráně firewall.</span><span class="sxs-lookup"><span data-stu-id="32e9c-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="32e9c-107">Podrobnosti najdete v tématu [Požadavky](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="32e9c-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="32e9c-108">Registrace může selhat, protože odchozí komunikace podléhá kontrole SSL přes síťovou vrstvu.</span><span class="sxs-lookup"><span data-stu-id="32e9c-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="32e9c-109">Ujistěte se, že jste ověřili nastavení oznámení pro Azure AD Connect Health, a zkontrolujte nastavení.</span><span class="sxs-lookup"><span data-stu-id="32e9c-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="32e9c-110">Informace o tom, jak nakonfigurovat nastavení oznámení pro oznámení o stavu služby Azure AD Connect, najdete v této [příručce.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="32e9c-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="32e9c-111">Další informace o sestavě synchronizace stavu připojení služby AAD a o tom, jak ji stáhnout, najdete v tématu Sestava synchronizace [na úrovni objektů](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="32e9c-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="32e9c-112">Řešení potíží s upozorněními na stav připojení služby AAD najdete v průvodci odstraňováním potíží s upozorněními na stav připojení [služby AAD a](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) nejčastějšími dotazy najdete v článku Časté otázky týkající se instalace služby [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="32e9c-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
