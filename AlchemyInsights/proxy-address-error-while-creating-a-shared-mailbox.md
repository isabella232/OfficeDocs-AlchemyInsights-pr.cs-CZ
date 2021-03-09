---
title: Chyba adresy proxy serveru při vytváření sdílené poštovní schránky
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568283"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="2b31d-102">Chyba adresy proxy serveru při vytváření poštovní schránky nebo jiného objektu s povoleným e-mailem</span><span class="sxs-lookup"><span data-stu-id="2b31d-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="2b31d-103">Pokud se vám při pokusu o vytvoření objektu s podporou e-mailu (poštovní schránka, sdílená poštovní schránka atd.) zobrazí chybová zpráva "Proxy adresa "SMTP:alias@domain.com" se už používá...", je e-mailová adresa, kterou jste vybrali, už pořízená jiným objektem ve vaší organizaci, který umožňuje e-mail.</span><span class="sxs-lookup"><span data-stu-id="2b31d-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="2b31d-104">Musíte najít uživatele, skupinu, sdílenou poštovní schránku nebo veřejnou složku s touto e-mailovou adresou a odstranit ji nebo změnit její e-mailovou adresu.</span><span class="sxs-lookup"><span data-stu-id="2b31d-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="2b31d-105">Potom můžete vytvořit nový objekt s povoleným e-mailem a pomocí odemkované e-mailové adresy.</span><span class="sxs-lookup"><span data-stu-id="2b31d-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="2b31d-106">K vyhledání použijte pole Hledat na domovské stránce.</span><span class="sxs-lookup"><span data-stu-id="2b31d-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="2b31d-107">Můžete ho také vyhledat pomocí následujícího příkazu Exchange Online PowerShellu:</span><span class="sxs-lookup"><span data-stu-id="2b31d-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="2b31d-108">Pokud nechcete odstranit existující e-mailovou adresu, zvolte novou e-mailovou adresu pro nový objekt, který vytváříte.</span><span class="sxs-lookup"><span data-stu-id="2b31d-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  