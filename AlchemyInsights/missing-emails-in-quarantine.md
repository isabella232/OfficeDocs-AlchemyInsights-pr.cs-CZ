---
title: Chybějící e-maily v karanténě
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569049"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="5a01e-102">Chybějící e-maily v karanténě"</span><span class="sxs-lookup"><span data-stu-id="5a01e-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="5a01e-103">Správci mohou [tyto zprávy zobrazit, uvolnit nebo odstranit.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="5a01e-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="5a01e-104">Chcete-li otevřít Centrum dodržování zabezpečení &, přejděte na [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="5a01e-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="5a01e-105">Chcete-li přímo otevřít stránku Karanténa, přejděte na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) položku .</span><span class="sxs-lookup"><span data-stu-id="5a01e-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="5a01e-106">Vyhledávat můžete podle následujících hodnot:</span><span class="sxs-lookup"><span data-stu-id="5a01e-106">You can search by the following values:</span></span>  

- <span data-ttu-id="5a01e-107">**ID zprávy**: Globálně jedinečný identifikátor zprávy.</span><span class="sxs-lookup"><span data-stu-id="5a01e-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="5a01e-108">Pokud v seznamu vyberete zprávu, zobrazí se **v** podokně informačního rámečku Podrobnosti v podokně **podrobností,** které se zobrazí.</span><span class="sxs-lookup"><span data-stu-id="5a01e-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="5a01e-109">Správci mohou pomocí [trasování zpráv](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) vyhledat zprávy a odpovídající hodnoty ID zprávy.</span><span class="sxs-lookup"><span data-stu-id="5a01e-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="5a01e-110">**E-mailová adresa odesílatele**: E-mailová adresa jednoho odesílatele.</span><span class="sxs-lookup"><span data-stu-id="5a01e-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="5a01e-111">**E-mailová adresa příjemce**: E-mailová adresa jednoho příjemce.</span><span class="sxs-lookup"><span data-stu-id="5a01e-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="5a01e-112">**Předmět**: Použijte celý předmět zprávy.</span><span class="sxs-lookup"><span data-stu-id="5a01e-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="5a01e-113">Hledání nerozeštkují malá a velká písmena.</span><span class="sxs-lookup"><span data-stu-id="5a01e-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="5a01e-114">Po zadání kritérií hledání klikněte na tlačítko Aktualizovat a ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** vyfiltrujte výsledky.  </span><span class="sxs-lookup"><span data-stu-id="5a01e-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="5a01e-115">Rutiny, které používáte k zobrazení a správě zpráv a souborů v karanténě, jsou:</span><span class="sxs-lookup"><span data-stu-id="5a01e-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="5a01e-116">Odstranit-KaranténaMessage</span><span class="sxs-lookup"><span data-stu-id="5a01e-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="5a01e-117">Export-KaranténaMessage</span><span class="sxs-lookup"><span data-stu-id="5a01e-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="5a01e-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="5a01e-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="5a01e-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Všimněte si, že tato rutina je určena pouze pro zprávy, nikoli pro soubory malwaru z ochrany ATP pro SharePoint Online, OneDrive pro firmy nebo Týmy.</span><span class="sxs-lookup"><span data-stu-id="5a01e-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="5a01e-120">Uvolnění-KaranténaMessage</span><span class="sxs-lookup"><span data-stu-id="5a01e-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)