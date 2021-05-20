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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539817"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="b70fa-102">Chybějící e-maily v karanténě"</span><span class="sxs-lookup"><span data-stu-id="b70fa-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="b70fa-103">Správci [můžou tyto zprávy zobrazit, uvolnit nebo odstranit.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="b70fa-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="b70fa-104">Pokud chcete otevřít Centrum & dodržování předpisů, přejděte na [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="b70fa-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="b70fa-105">Pokud chcete stránku Karanténa otevřít přímo, přejděte na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="b70fa-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="b70fa-106">Můžete hledat podle následujících hodnot:</span><span class="sxs-lookup"><span data-stu-id="b70fa-106">You can search by the following values:</span></span>  

- <span data-ttu-id="b70fa-107">**ID zprávy:** Globálně jedinečný identifikátor zprávy.</span><span class="sxs-lookup"><span data-stu-id="b70fa-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="b70fa-108">Pokud v seznamu vyberete zprávu, zobrazí se **hodnota ID zprávy** v podokně podrobností, které se zobrazí. </span><span class="sxs-lookup"><span data-stu-id="b70fa-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="b70fa-109">Správci mohou pomocí [sledování zpráv](/microsoft-365/security/office-365-security/message-trace-scc) najít zprávy a odpovídající hodnoty ID zprávy.</span><span class="sxs-lookup"><span data-stu-id="b70fa-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="b70fa-110">**E-mailová adresa** odesílatele: E-mailová adresa jednoho odesílatele.</span><span class="sxs-lookup"><span data-stu-id="b70fa-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="b70fa-111">**E-mailová adresa příjemce:** E-mailová adresa jednoho příjemce.</span><span class="sxs-lookup"><span data-stu-id="b70fa-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="b70fa-112">**Předmět:** Použijte celý předmět zprávy.</span><span class="sxs-lookup"><span data-stu-id="b70fa-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="b70fa-113">Při hledání se rozlišují malá a velká písmena.</span><span class="sxs-lookup"><span data-stu-id="b70fa-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="b70fa-114">Po zadání kritérií hledání klikněte na tlačítko Aktualizovat aktualizovat a ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  vyfiltrujte výsledky.</span><span class="sxs-lookup"><span data-stu-id="b70fa-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="b70fa-115">Rutiny, které používáte k zobrazení a správě zpráv a souborů v karanténě, jsou:</span><span class="sxs-lookup"><span data-stu-id="b70fa-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="b70fa-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="b70fa-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="b70fa-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="b70fa-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="b70fa-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="b70fa-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="b70fa-119">[Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Tato rutina je jenom pro zprávy, ne pro soubory malwaru z programu Microsoft Defender pro Office 365 pro SharePoint Online, OneDrive pro firmy nebo Teams.</span><span class="sxs-lookup"><span data-stu-id="b70fa-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="b70fa-120">Zpráva o uvolnění do karantény</span><span class="sxs-lookup"><span data-stu-id="b70fa-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)