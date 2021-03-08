---
title: Konfigurace šifrování zpráv pro hybridní prostředí
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523986"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="6282e-102">Konfigurace šifrování zpráv pro hybridní prostředí</span><span class="sxs-lookup"><span data-stu-id="6282e-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="6282e-103">V hybridních prostředích Exchange mohou místní uživatelé posílat šifrované e-maily pomocí šifrování zpráv Office (OME) jenom v případě, že jsou e-maily směrované přes Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="6282e-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="6282e-104">Při šifrování e-mailů pomocí OME postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="6282e-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="6282e-105">K nastavení [hybridního prostředí použijte](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) Průvodce hybridní konfigurací.</span><span class="sxs-lookup"><span data-stu-id="6282e-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="6282e-106">K nastavení šifrování nejsou potřeba žádné zvláštní kroky.</span><span class="sxs-lookup"><span data-stu-id="6282e-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="6282e-107">[Nastavte pravidla toku pošty pro šifrování](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) běžným způsobem.</span><span class="sxs-lookup"><span data-stu-id="6282e-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


