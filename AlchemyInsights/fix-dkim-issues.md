---
title: Oprava problémů s nastavením DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744943"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="6d0ad-102">Oprava problémů s nastavením DKIM</span><span class="sxs-lookup"><span data-stu-id="6d0ad-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="6d0ad-103">Pokud máte problémy s povolením DKIM pro vaši vlastní doménu, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="6d0ad-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="6d0ad-104">Většina problémů s nastavením DKIM souvisí s nesprávnými záznamy DNS.</span><span class="sxs-lookup"><span data-stu-id="6d0ad-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="6d0ad-105">Ověřte, jestli je záznam CNAME DKIM (**ne** záznam TXT) správně naformátovaný.</span><span class="sxs-lookup"><span data-stu-id="6d0ad-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="6d0ad-106">Další informace najdete v tomto [tématu](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="6d0ad-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="6d0ad-107">Po vytvoření nebo aktualizaci záznamů DNS DKIM u hostitelské služby DNS pro vaši doménu (obvykle u doménového registrátora) Počkejte na rozšíření záznamů DNS.</span><span class="sxs-lookup"><span data-stu-id="6d0ad-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="6d0ad-108">Pokud v centru pro správu nemůžete vytvořit záznamy DNS DKIM, můžete je nahradit \<CustomDomain\> vlastní doménou (třeba contoso.com) a spustit tento příkaz v [PowerShellu Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="6d0ad-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
