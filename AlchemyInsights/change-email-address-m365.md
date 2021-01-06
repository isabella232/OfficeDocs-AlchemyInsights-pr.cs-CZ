---
title: Změna e-mailové adresy skupiny Microsoftu 365 nebo Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756550"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="0520b-102">Změna e-mailové adresy skupiny Microsoftu 365 nebo Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0520b-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="0520b-103">E-mailovou adresu skupiny Microsoftu 365 nebo Microsoft Teams můžete změnit v [Centru pro správu Microsoftu 365](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="0520b-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="0520b-104">Stačí vybrat skupinu a pak vybrat @upravit e-mailovou adresu.</span><span class="sxs-lookup"><span data-stu-id="0520b-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="0520b-105">Ke změně primární SMTP adresy skupiny Microsoftu 365 nebo Teams můžete použít i následující příkaz EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="0520b-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="0520b-106">Příklad:</span><span class="sxs-lookup"><span data-stu-id="0520b-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
