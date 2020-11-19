---
title: Odvolání nebo nahrazení e-mailové zprávy
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353499"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="cde86-102">Odvolání nebo nahrazení e-mailové zprávy v Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="cde86-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="cde86-103">Můžete **odvolat pouze zprávy, které jsou posílány lidem ve vaší organizaci**.</span><span class="sxs-lookup"><span data-stu-id="cde86-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="cde86-104">Pokud je třeba zpráva odeslána na adresu Gmail, nemůžete ji odvolat.</span><span class="sxs-lookup"><span data-stu-id="cde86-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="cde86-105">**Do počítače můžete odvolat pouze zprávy poslané z Outlooku**.</span><span class="sxs-lookup"><span data-stu-id="cde86-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="cde86-106">Pokud uživatel pošle zprávu pomocí Outlooku pro Mac nebo Outlooku na webu, nemůžete ho odvolat.</span><span class="sxs-lookup"><span data-stu-id="cde86-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="cde86-107">Jako správce klienta můžete **zprávy odvolat jménem uživatelů pomocí PowerShellu** (Další informace najdete v tématu [hledání a odstranění e-mailových zpráv](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="cde86-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="cde86-108">V centru pro správu se nedají odvolat zprávy.</span><span class="sxs-lookup"><span data-stu-id="cde86-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="cde86-109">Další informace najdete v tématu Vyhledání a odstranění e-mailových zpráv v organizaci.</span><span class="sxs-lookup"><span data-stu-id="cde86-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="cde86-110">**Odvolání nebo nahrazení odeslané e-mailové zprávy**</span><span class="sxs-lookup"><span data-stu-id="cde86-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="cde86-111">V podokně složek na levé straně okna Outlooku zvolte složku Odeslaná pošta.</span><span class="sxs-lookup"><span data-stu-id="cde86-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="cde86-112">Otevřete zprávu, kterou chcete odvolat.</span><span class="sxs-lookup"><span data-stu-id="cde86-112">Open the message that you want to recall.</span></span> <span data-ttu-id="cde86-113">Zprávu otevřete poklikáním.</span><span class="sxs-lookup"><span data-stu-id="cde86-113">You must double-click to open the message.</span></span> <span data-ttu-id="cde86-114">Výběr zprávy, aby se zobrazila v podokně čtení, neumožňuje odvolat zprávu.</span><span class="sxs-lookup"><span data-stu-id="cde86-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="cde86-115">Na kartě zpráva vyberte **Akce**  >  **odvolat zprávu**.</span><span class="sxs-lookup"><span data-stu-id="cde86-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="cde86-116">Zvolte **Odstranit nepřečtené kopie této zprávy** nebo **Odstranit nepřečtené kopie a nahradit je novou zprávou a** pak vyberte **OK**.</span><span class="sxs-lookup"><span data-stu-id="cde86-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="cde86-117">Pokud posíláte náhradní zprávu, napište zprávu a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="cde86-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="cde86-118">Úspěšné nebo neúspěšné odvolání zprávy závisí na nastavení příjemců v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="cde86-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="cde86-119">Další informace, včetně toho, jak zkontrolovat odvolat, najdete v tématu [odvolání nebo nahrazení e-mailové zprávy, kterou jste odeslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="cde86-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="cde86-120">Pokud chcete **_Vyhledat a odstranit e-mailové zprávy ve vaší organizaci_**, je jednodušší, když jste globální správce. Pokud nejste globální správce, musíte účet přidat do skupiny rolí správce eDiscovery nebo do role pro správu hledání dodržování předpisů.</span><span class="sxs-lookup"><span data-stu-id="cde86-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="cde86-121">Pokud chcete odstranit zprávy, musíte se připojit ke skupině rolí Správa organizace nebo k roli pro správu vyhledávání a mazání.</span><span class="sxs-lookup"><span data-stu-id="cde86-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="cde86-122">Oprávnění k těmto rolím se přiřazují v [Centru zabezpečení & dodržování předpisů](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="cde86-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="cde86-123">[Vytvořte vyhledávání obsahu](https://docs.microsoft.com/microsoft-365/compliance/content-search) a vyhledejte zprávu, která se má odstranit.</span><span class="sxs-lookup"><span data-stu-id="cde86-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="cde86-124">[Připojení k PowerShellu centra dodržování předpisů &](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="cde86-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="cde86-125">Pokud používáte VÍCEFAKTOROVÉ ověřování (Multi-Factor Authentication), najdete další informace v tématu [připojení k webu Centrum pro kompatibilitu se systémem & 365 pomocí vícefaktorového ověřování](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="cde86-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
