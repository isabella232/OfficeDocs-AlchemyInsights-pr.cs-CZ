---
title: Zpráva o tom, že v Centru zabezpečení nebyla nalezena žádná předplatná
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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713412"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="63cb1-102">Zpráva o tom, že v Centru zabezpečení nebyla nalezena žádná předplatná</span><span class="sxs-lookup"><span data-stu-id="63cb1-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="63cb1-103">Pokud se při přístupu k Centru zabezpečení v programu Microsoft Defender zobrazí zpráva "Nenašla se žádná předplatná", znamená to, že služba Azure Active Directory (AAD) použitá k přihlášení uživatele k portálu nemá licenci Microsoft Defenderu atp.</span><span class="sxs-lookup"><span data-stu-id="63cb1-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="63cb1-104">Licence na Windows E5 a Office E5 jsou samostatné licence.</span><span class="sxs-lookup"><span data-stu-id="63cb1-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="63cb1-105">Otevřete případ podpory, pokud byla licence zakoupena, ale nebyla zřízena pro tuto instanci služby AAD.</span><span class="sxs-lookup"><span data-stu-id="63cb1-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="63cb1-106">Máte buď:</span><span class="sxs-lookup"><span data-stu-id="63cb1-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="63cb1-107">Možný problém s zřizováním licencí.</span><span class="sxs-lookup"><span data-stu-id="63cb1-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="63cb1-108">Neúmyslně jste zřizaci licence jinému účtu Microsoft AAD, než se používá k ověřování ve službě.</span><span class="sxs-lookup"><span data-stu-id="63cb1-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>