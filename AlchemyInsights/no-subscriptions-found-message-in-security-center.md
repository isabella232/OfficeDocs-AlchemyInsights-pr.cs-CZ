---
title: V Centru zabezpečení nebyla nalezena žádná zpráva o předplatných.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544101"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="6dd7f-102">V Centru zabezpečení nebyla nalezena žádná zpráva o předplatných.</span><span class="sxs-lookup"><span data-stu-id="6dd7f-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="6dd7f-103">Pokud se při Centrum zabezpečení v programu Microsoft Defender zobrazí zpráva o tom, že se nenašla žádná předplatná, znamená to, že Azure Active Directory (AAD), který se používá k přihlášení uživatele k portálu, nemá Microsoft Defender ATP licenci.</span><span class="sxs-lookup"><span data-stu-id="6dd7f-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="6dd7f-104">Licence Windows E5 a Office E5 jsou samostatné licence.</span><span class="sxs-lookup"><span data-stu-id="6dd7f-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="6dd7f-105">Otevřete případ podpory, pokud byla licence zakoupena, ale nebyla zřízena pro tuto instanci služby AAD.</span><span class="sxs-lookup"><span data-stu-id="6dd7f-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="6dd7f-106">Buď máte:</span><span class="sxs-lookup"><span data-stu-id="6dd7f-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="6dd7f-107">Možný problém se zřizováním licencí.</span><span class="sxs-lookup"><span data-stu-id="6dd7f-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="6dd7f-108">Neúmyslně jste zřásekli licenci na jinou službu Microsoft AAD, než která se používá k ověřování ve službě.</span><span class="sxs-lookup"><span data-stu-id="6dd7f-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>