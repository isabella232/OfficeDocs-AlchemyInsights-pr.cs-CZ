---
title: Řešení problémů s doručováním e-mailů do veřejných složek s podporou pošty
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
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677921"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="4f1ae-102">Řešení problémů s doručováním e-mailů do veřejných složek s podporou pošty</span><span class="sxs-lookup"><span data-stu-id="4f1ae-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="4f1ae-103">Pokud externí odesílatelé nemůžou posílat zprávy do vaší poštovní složky s povoleným e-mailem a odesílatelé obdrží chybu: **nejde najít (550 5.4.1)**, ověřte, že e-mailová doména pro veřejnou složku je nakonfigurovaná jako vnitřní doména přenosu místo autoritativní domény:</span><span class="sxs-lookup"><span data-stu-id="4f1ae-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="4f1ae-104">Otevřete [Centrum pro správu Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="4f1ae-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="4f1ae-105">Přejděte do **Mail flow** \> **domény přijatý**přenos, vyberte přijatou doménu a klikněte na **Upravit**.</span><span class="sxs-lookup"><span data-stu-id="4f1ae-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="4f1ae-106">Na stránce vlastnosti, která se otevře, pokud je typ domény nastaven na **autoritativní**, změňte hodnotu na **interní relé** a klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="4f1ae-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="4f1ae-107">Pokud externí odesílatelé obdrží chybu, **kterou nemáte oprávnění (550 5.7.13)**, spusťte následující příkaz v [PowerShellu online pro Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a zobrazte oprávnění pro anonymní uživatele ve veřejné složce:</span><span class="sxs-lookup"><span data-stu-id="4f1ae-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="4f1ae-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Třeba `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="4f1ae-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="4f1ae-109">Pokud chcete povolit externím uživatelům posílání e-mailů do této veřejné složky, přidejte anonymnímu uživateli oprávnění k přístupu k CreateItems.</span><span class="sxs-lookup"><span data-stu-id="4f1ae-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="4f1ae-110">Třeba `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="4f1ae-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
