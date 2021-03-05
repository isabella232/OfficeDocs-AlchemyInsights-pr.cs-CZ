---
title: Problém se stavem služby AAD Connect
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481151"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="fb13a-102">Problém se stavem služby AAD Connect</span><span class="sxs-lookup"><span data-stu-id="fb13a-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="fb13a-103">Ujistěte se, že máte oprávnění k provádění operace.</span><span class="sxs-lookup"><span data-stu-id="fb13a-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="fb13a-104">Ve výchozím nastavení mají přístup globální správci.</span><span class="sxs-lookup"><span data-stu-id="fb13a-104">Global Admins have access by default.</span></span> <span data-ttu-id="fb13a-105">Navíc můžete pomocí ovládacího prvku přístupu [založeného na](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) rolích delegovat oprávnění k registraci přispěvatele.</span><span class="sxs-lookup"><span data-stu-id="fb13a-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="fb13a-106">Ujistěte se, že jsou povolené požadované koncové body a nezablokují se kvůli bráně firewall.</span><span class="sxs-lookup"><span data-stu-id="fb13a-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="fb13a-107">Podrobnosti najdete v části [požadavky.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="fb13a-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="fb13a-108">Registrace může selhat, pokud se odchozí komunikace podrobuje kontrole SSL síťové vrstvě.</span><span class="sxs-lookup"><span data-stu-id="fb13a-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="fb13a-109">Zkontrolujte, že jste ověřili nastavení oznámení pro Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="fb13a-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="fb13a-110">Zkontrolujte prosím nastavení.</span><span class="sxs-lookup"><span data-stu-id="fb13a-110">Please review your setting.</span></span> <span data-ttu-id="fb13a-111">Tento [průvodce vám](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) pomůže pochopit, jak nakonfigurovat nastavení oznámení pro upozornění na stav služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="fb13a-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="fb13a-112">Další informace o sestavě synchronizace služby AAD Connect Health a o tom, jak ji stáhnout, najdete v [sestavě synchronizace na úrovni objektů.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="fb13a-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="fb13a-113">Pokud chcete vyřešit upozornění na stav služby AAD Connect, postupujte podle pokynů průvodce pro řešení potíží s upozorněními na aktualizace dat [služby AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) a nejčastějšími otázkami k instalaci najdete v článku Časté otázky týkající se instalace služby [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="fb13a-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
