---
title: Konfigurace ochrany proti dlp koncového bodu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/03/2020
ms.locfileid: "46554923"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="deac9-102">Konfigurace ochrany proti dlp koncového bodu</span><span class="sxs-lookup"><span data-stu-id="deac9-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="deac9-103">Microsoft Endpoint DLP umožňuje rozšířit ochranu ochrany proti dlp a monitorování schopnost citlivých informací na zařízeních s Windows 10.</span><span class="sxs-lookup"><span data-stu-id="deac9-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="deac9-104">Po připojení zařízení do správy zařízení můžete vytvořit zásady ochrany před únikem přístupu k vynucení ochranných akcí na položkách.</span><span class="sxs-lookup"><span data-stu-id="deac9-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="deac9-105">Průzkumník aktivit lze použít ke sledování aktivity pro citlivé položky.</span><span class="sxs-lookup"><span data-stu-id="deac9-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="deac9-106">Další informace najdete [v tématu Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="deac9-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="deac9-107">Jak začít s koncovýmpointem DLP:</span><span class="sxs-lookup"><span data-stu-id="deac9-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="deac9-108">Ujistěte se, že máte příslušné licencování skladových žim/předplatných.</span><span class="sxs-lookup"><span data-stu-id="deac9-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="deac9-109">Další informace najdete v [tématu Licencování skladových položek a předplatných](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="deac9-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="deac9-110">Zkontrolujte oprávnění potřebná k povolení správy zařízení, přístupu na stránku registrace nebo zapnutí/vypnutí monitorování zařízení.</span><span class="sxs-lookup"><span data-stu-id="deac9-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="deac9-111">Další informace naleznete v [tématu Oprávnění](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="deac9-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="deac9-112">Integrované zařízení do správy zařízení podle postupu registrace zařízení.</span><span class="sxs-lookup"><span data-stu-id="deac9-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="deac9-113">Pokud vám v **nastavení**dodržování předpisů M365 chybí možnost Registrace zařízení (náhled), potvrďte, že máte příslušnou licenci a oprávnění uvedená výše.</span><span class="sxs-lookup"><span data-stu-id="deac9-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="deac9-114">Další informace naleznete [v tématu Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="deac9-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="deac9-115">Vytvořte zásady ochrany před únikem bodů ochrany před únikem od ochrany před únikem od zařízení a ochranu před citlivými položkami.</span><span class="sxs-lookup"><span data-stu-id="deac9-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="deac9-116">Další informace naleznete v [tématu scénáře zásad DLP koncového bodu](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="deac9-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="deac9-117">Další informace o ochraně dlp koncových bodů aplikace Microsoft Endpoint [najdete v tématu Informace o prevenci ztráty dat koncových bodů Microsoft 365 (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="deac9-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>