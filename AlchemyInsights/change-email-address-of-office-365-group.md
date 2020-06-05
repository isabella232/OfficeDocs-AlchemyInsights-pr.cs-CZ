---
title: Změna e-mailové adresy skupiny Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580650"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="716d9-102">Změna e-mailové adresy skupiny Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="716d9-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="716d9-103">E-mailovou adresu skupiny Microsoft 365 můžete změnit pomocí Centra pro správu.</span><span class="sxs-lookup"><span data-stu-id="716d9-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="716d9-104">Stačí vybrat skupinu a vybrat @edit e-mailovou adresu.</span><span class="sxs-lookup"><span data-stu-id="716d9-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="716d9-105">Pomocí následujícího příkazu EXO PowerShell můžete také změnit primární adresu SMTP skupiny Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="716d9-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="716d9-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="716d9-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="716d9-107">Příklad:</span><span class="sxs-lookup"><span data-stu-id="716d9-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
