---
title: Identifikační řetězec prohlížeče Microsoft Edge (plocha)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677055"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="408bb-102">Identifikační řetězec prohlížeče Microsoft Edge (plocha)</span><span class="sxs-lookup"><span data-stu-id="408bb-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="408bb-103">Pomocí řetězců User Agent (UA) můžete zjistit, jaká verze konkrétního prohlížeče se používá v určitém operačním systému.</span><span class="sxs-lookup"><span data-stu-id="408bb-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="408bb-104">Podobně jako jiné prohlížeče Microsoft Edge tyto informace začleňuje do hlavičky User-Agent "HTTP, kdykoli to vytvoří žádost na web.</span><span class="sxs-lookup"><span data-stu-id="408bb-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="408bb-105">Informace o verzi do prohlížeče mohou být přístupné prostřednictvím JavaScriptu pomocí dotazu na hodnotu "Navigator. userAgent".</span><span class="sxs-lookup"><span data-stu-id="408bb-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="408bb-106">Doporučujeme, aby vývojáři webu používali zjišťování funkcí všude, kde je to možné, ke zlepšení udržení kódu, omezení nezávisle na kódu a eliminace rizika v případě v budoucích aktualizacích řetězců systému UA.</span><span class="sxs-lookup"><span data-stu-id="408bb-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="408bb-107">Další informace najdete v tématu [Microsoft Edge-identifikační řetězec (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="408bb-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>