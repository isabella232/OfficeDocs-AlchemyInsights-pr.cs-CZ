---
title: Odchozí e-mail do složky Nevyžádaná pošta
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769176"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="83077-102">Odchozí e-mail do složky Nevyžádaná pošta</span><span class="sxs-lookup"><span data-stu-id="83077-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="83077-103">Pokud vidíte odchozí zprávy označené jako nevyžádané, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="83077-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="83077-104">Pokud jste to ještě neudělali, zvažte [konfiguraci odchozích oznámení zásad nevyžádané pošty](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="83077-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="83077-105">Pomocí [sledování zpráv](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) můžete zjistit, jestli má odchozí zpráva v hodnotě události **Nevyžádaná pošta** s dalšími podrobnostmi: **Využijte vysoké rizikové zdroje**.</span><span class="sxs-lookup"><span data-stu-id="83077-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="83077-106">U těchto zpráv můžete zkontrolovat obsah zprávy a zjistit, co se považuje za spam.</span><span class="sxs-lookup"><span data-stu-id="83077-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="83077-107">Podpisy mohou někdy způsobovat problémy s mnoha uživateli.</span><span class="sxs-lookup"><span data-stu-id="83077-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="83077-108">Pokud máte několik příkladů legitimních odchozích zpráv, které jsou označené jako nevyžádaná pošta, otevřete lístek podpory a požádejte agenta podpory o odeslání zpráv jako falešných pozitivních pro naše analytiky nevyžádané pošty.</span><span class="sxs-lookup"><span data-stu-id="83077-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="83077-109">Připravte se na poskytování ukázkových zpráv obsahujících všechna záhlaví zpráv.</span><span class="sxs-lookup"><span data-stu-id="83077-109">Be prepared to provide sample messages that include all message headers.</span></span>
