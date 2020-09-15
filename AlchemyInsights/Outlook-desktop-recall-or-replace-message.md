---
title: Stažení nebo nahrazení e-mailové zprávy v Outlooku
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663983"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="51199-102">Odvolání nebo nahrazení e-mailové zprávy Outlooku</span><span class="sxs-lookup"><span data-stu-id="51199-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="51199-103">Jako správce můžete **zprávy odvolat jménem uživatelů pomocí PowerShellu**.</span><span class="sxs-lookup"><span data-stu-id="51199-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="51199-104">V centru pro správu se nedají odvolat zprávy.</span><span class="sxs-lookup"><span data-stu-id="51199-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="51199-105">Můžete **odvolat pouze zprávy, které jsou posílány lidem ve vaší organizaci**.</span><span class="sxs-lookup"><span data-stu-id="51199-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="51199-106">Pokud byla zpráva odeslána na adresu Gmail, například ji nemůžete odvolat.</span><span class="sxs-lookup"><span data-stu-id="51199-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="51199-107">**Do počítače můžete odvolat pouze zprávy odeslané z outlooku 2016**.</span><span class="sxs-lookup"><span data-stu-id="51199-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="51199-108">Pokud uživatel pošle zprávu pomocí Outlooku pro Mac nebo Outlooku na webu, nemůžete ho odvolat.</span><span class="sxs-lookup"><span data-stu-id="51199-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="51199-109">Odvolání nebo nahrazení e-mailové zprávy:</span><span class="sxs-lookup"><span data-stu-id="51199-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="51199-110">V podokně složek na levé straně okna Outlooku vyberte složku Odeslaná pošta.</span><span class="sxs-lookup"><span data-stu-id="51199-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="51199-111">Poklikejte na zprávu, kterou chcete odvolat, a otevřete ji.</span><span class="sxs-lookup"><span data-stu-id="51199-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="51199-112">Vyberte kartu **zpráva** a pak vyberte **Akce**Odvolejte  >  **tuto zprávu**.</span><span class="sxs-lookup"><span data-stu-id="51199-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="51199-113">Vyberte **Odstranit nepřečtené kopie této zprávy** nebo **Odstranit nepřečtené kopie a nahradit je novou zprávou**a pak vyberte **OK**.</span><span class="sxs-lookup"><span data-stu-id="51199-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="51199-114">Pokud posíláte náhradní zprávu, napište zprávu a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="51199-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="51199-115">Úspěšné nebo neúspěšné odvolání zprávy závisí na nastaveních příjemce v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="51199-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="51199-116">Postup pro kontrolu odvolání najdete v [tomto článku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="51199-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="51199-117">Vyhledání a odstranění e-mailových zpráv v organizaci</span><span class="sxs-lookup"><span data-stu-id="51199-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="51199-118">Pokud nejste globálním správcem, musí být váš účet přidán do role správce eDiscovery nebo role pro správu vyhledávání dodržování předpisů pro hledání zpráv.</span><span class="sxs-lookup"><span data-stu-id="51199-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="51199-119">Pokud chcete odstranit zprávy, musíte se připojit ke skupině rolí Správa organizace nebo k roli pro správu vyhledávání a mazání.</span><span class="sxs-lookup"><span data-stu-id="51199-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="51199-120">Oprávnění pro tyto role jsou přiřazena v [Centru zabezpečení a dodržování předpisů](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="51199-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="51199-121">[Vytvořte vyhledávání obsahu](https://docs.microsoft.com/microsoft-365/compliance/content-search) a vyhledejte zprávu, která se má odstranit.</span><span class="sxs-lookup"><span data-stu-id="51199-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="51199-122">[Připojení k PowerShellu pro zabezpečení a dodržování předpisů](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="51199-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="51199-123">Pokud používáte vícefaktorové ověřování, přečtěte si článek [připojení k prostředí PowerShell pro zabezpečení a dodržování předpisů pro systém Microsoft 365 pomocí vícefaktorového ověřování](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="51199-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>