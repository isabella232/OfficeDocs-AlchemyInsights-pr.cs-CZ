---
title: 126 Při získání poštovní schránky se v aplikaci OWA nenašla chyba?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426655"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="75981-102">Zobrazí se v Outlooku na webu chyba, že se poštovní schránka nenašla?</span><span class="sxs-lookup"><span data-stu-id="75981-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="75981-103">Pokud používáte Outlook na webu **a** zobrazí se chyba Poštovní schránka, účet, který jste použili pro připojení k Outlooku na webu, nemá licenci Exchange Online, a proto není k účtu přidružená žádná poštovní schránka.</span><span class="sxs-lookup"><span data-stu-id="75981-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="75981-104">Správce může přiřadit licenci k vašemu účtu takto:</span><span class="sxs-lookup"><span data-stu-id="75981-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="75981-105">Otevřete  [Centrum pro správu Microsoftu 365](https://portal.office.com/adminportal/home#/homepage)  a v části Uživatelé přejděte na Aktivní uživatelé a vyberte uživatele, který chybu vidí.</span><span class="sxs-lookup"><span data-stu-id="75981-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="75981-106">Na stránce uživatele, která se  otevře, přejděte do části  Licence a aplikace, vyberte příslušnou hodnotu Umístění a přiřaďte licenci obsahující Exchange Online (rozbalte licenci a zobrazte její podrobnosti).</span><span class="sxs-lookup"><span data-stu-id="75981-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="75981-107">Až skončíte, klikněte na **Uložit změny**.</span><span class="sxs-lookup"><span data-stu-id="75981-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="75981-108">V některých případech, pokud je licence už přiřazená k uživatelskému účtu, pomáhá odebrání a opětovné přiřazení licence problém vyřešit a zajistit jeho správné zřízení v systému:</span><span class="sxs-lookup"><span data-stu-id="75981-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="75981-109">Zkontrolujte, jestli jsou vaše předplatná M365 Exchange Online (a další, pokud máte) aktuální a ještě nedávno nevyšly platnosti.</span><span class="sxs-lookup"><span data-stu-id="75981-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="75981-110">Po ověření, že platnost vašeho předplatného nevy vypršela a byla přiřazena platná licence k uživatelskému účtu, může zřízení licence trvat až 24 hodin, takže budete muset počkat, až se problém vyřeší.</span><span class="sxs-lookup"><span data-stu-id="75981-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="75981-111">Další informace najdete v tématu [Přiřazení a správa licencí](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span><span class="sxs-lookup"><span data-stu-id="75981-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>