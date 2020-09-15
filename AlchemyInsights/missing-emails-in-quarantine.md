---
title: Chybějící e-maily v karanténě
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673707"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="0fbd1-102">Chybějící e-maily v karanténě</span><span class="sxs-lookup"><span data-stu-id="0fbd1-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="0fbd1-103">Správci můžou [tyto zprávy zobrazit, uvolnit nebo odstranit.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="0fbd1-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="0fbd1-104">Pokud chcete otevřít Centrum pro dodržování předpisů &, přejděte na [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="0fbd1-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="0fbd1-105">Pokud chcete stránku karantény otevřít přímo, přejděte na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="0fbd1-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="0fbd1-106">Můžete hledat podle následujících hodnot:</span><span class="sxs-lookup"><span data-stu-id="0fbd1-106">You can search by the following values:</span></span>  

- <span data-ttu-id="0fbd1-107">**ID zprávy**: globálně jedinečný identifikátor zprávy.</span><span class="sxs-lookup"><span data-stu-id="0fbd1-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="0fbd1-108">Pokud v seznamu vyberete zprávu, zobrazí se v zobrazeném podokně informační  **seznam s**  **podrobnostmi**  .</span><span class="sxs-lookup"><span data-stu-id="0fbd1-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="0fbd1-109">Správci můžou pomocí [sledování zpráv](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) najít zprávy a odpovídající hodnoty ID zprávy.</span><span class="sxs-lookup"><span data-stu-id="0fbd1-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="0fbd1-110">**E-mailová adresa odesílatele**: e-mailová adresa jednoho odesílatele</span><span class="sxs-lookup"><span data-stu-id="0fbd1-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="0fbd1-111">**E-mailová adresa příjemce**: e-mailová adresa jednoho příjemce</span><span class="sxs-lookup"><span data-stu-id="0fbd1-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="0fbd1-112">**Předmět**: použijte celý předmět zprávy.</span><span class="sxs-lookup"><span data-stu-id="0fbd1-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="0fbd1-113">V hledání se nerozlišují malá a velká písmena.</span><span class="sxs-lookup"><span data-stu-id="0fbd1-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="0fbd1-114">Po zadání kritérií vyhledávání kliknutím na tlačítko ![ aktualizovat ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **aktualizujte** výsledky.  </span><span class="sxs-lookup"><span data-stu-id="0fbd1-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="0fbd1-115">K zobrazení a správě zpráv a souborů v karanténě slouží rutiny:</span><span class="sxs-lookup"><span data-stu-id="0fbd1-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="0fbd1-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="0fbd1-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="0fbd1-117">Export – QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="0fbd1-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="0fbd1-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="0fbd1-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="0fbd1-119">[Náhled – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Tato rutina je jenom pro zprávy, ne pro soubory malwaru z ATP pro SharePoint Online, OneDrive pro firmy nebo týmy.</span><span class="sxs-lookup"><span data-stu-id="0fbd1-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="0fbd1-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="0fbd1-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)