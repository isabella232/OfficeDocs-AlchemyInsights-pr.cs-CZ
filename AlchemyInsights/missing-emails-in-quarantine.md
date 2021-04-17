---
title: Chybějící e-maily v karanténě
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831727"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="609f7-102">Chybějící e-maily v karanténě"</span><span class="sxs-lookup"><span data-stu-id="609f7-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="609f7-103">Správci [můžou tyto zprávy zobrazit, uvolnit nebo odstranit.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="609f7-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="609f7-104">Pokud chcete otevřít Centrum & dodržování předpisů, přejděte na [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="609f7-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="609f7-105">Pokud chcete stránku Karanténa otevřít přímo, přejděte na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="609f7-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="609f7-106">Můžete hledat podle následujících hodnot:</span><span class="sxs-lookup"><span data-stu-id="609f7-106">You can search by the following values:</span></span>  

- <span data-ttu-id="609f7-107">**ID zprávy:** Globálně jedinečný identifikátor zprávy.</span><span class="sxs-lookup"><span data-stu-id="609f7-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="609f7-108">Pokud v seznamu vyberete zprávu, zobrazí se **hodnota ID zprávy** v podokně podrobností, které se zobrazí. </span><span class="sxs-lookup"><span data-stu-id="609f7-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="609f7-109">Správci mohou pomocí [sledování zpráv](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) najít zprávy a odpovídající hodnoty ID zprávy.</span><span class="sxs-lookup"><span data-stu-id="609f7-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="609f7-110">**E-mailová adresa** odesílatele: E-mailová adresa jednoho odesílatele.</span><span class="sxs-lookup"><span data-stu-id="609f7-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="609f7-111">**E-mailová adresa příjemce:** E-mailová adresa jednoho příjemce.</span><span class="sxs-lookup"><span data-stu-id="609f7-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="609f7-112">**Předmět:** Použijte celý předmět zprávy.</span><span class="sxs-lookup"><span data-stu-id="609f7-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="609f7-113">Při hledání se rozlišují malá a velká písmena.</span><span class="sxs-lookup"><span data-stu-id="609f7-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="609f7-114">Po zadání kritérií hledání klikněte na tlačítko Aktualizovat aktualizovat a ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  vyfiltrujte výsledky.  </span><span class="sxs-lookup"><span data-stu-id="609f7-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="609f7-115">Rutiny, které používáte k zobrazení a správě zpráv a souborů v karanténě, jsou:</span><span class="sxs-lookup"><span data-stu-id="609f7-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="609f7-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="609f7-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="609f7-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="609f7-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="609f7-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="609f7-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="609f7-119">[Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Tato rutina je jenom pro zprávy, ne pro soubory malwaru z atp pro SharePoint Online, OneDrive pro firmy nebo Teams.</span><span class="sxs-lookup"><span data-stu-id="609f7-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="609f7-120">Zpráva o uvolnění do karantény</span><span class="sxs-lookup"><span data-stu-id="609f7-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)