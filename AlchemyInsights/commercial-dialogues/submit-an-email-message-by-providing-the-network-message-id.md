---
title: Odeslání e-mailové zprávy poskytnutím ID síťové zprávy
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744238"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="3024f-102">Odeslání e-mailové zprávy poskytnutím ID síťové zprávy</span><span class="sxs-lookup"><span data-stu-id="3024f-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="3024f-103">V **plovoucím seznamu Nové** odeslání vyberte **E-mail** a **ID síťové zprávy**.</span><span class="sxs-lookup"><span data-stu-id="3024f-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="3024f-104">Pokud chcete v Outlooku najít ID zprávy pro e-mailovou zprávu, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="3024f-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="3024f-105">Poklikejte na e-mailovou zprávu a otevřete ji.</span><span class="sxs-lookup"><span data-stu-id="3024f-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="3024f-106">Vyberte **Vlastnosti**  >  **souboru**.</span><span class="sxs-lookup"><span data-stu-id="3024f-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="3024f-107">Otevřete Poznámkový blok nebo prázdný wordový dokument a pak  zkopírujte a vložte obsah, který se nachází v poli Záhlaví internetu, do otevřeného dokumentu, aby byl lépe přehlednější.</span><span class="sxs-lookup"><span data-stu-id="3024f-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="3024f-108">Vyhledejte **pole X-MS-Exchange-Organization-Network-Message-Id.**</span><span class="sxs-lookup"><span data-stu-id="3024f-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="3024f-109">Hodnota za **:** je ID, které potřebujete pro odeslání.</span><span class="sxs-lookup"><span data-stu-id="3024f-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="3024f-110">Pokud **se e-mail** v části Příjemci ve složce nevyžádané pošty pro všechny příjemce tohoto e-mailu došla, zvolte **Vybrat vše**.</span><span class="sxs-lookup"><span data-stu-id="3024f-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="3024f-111">Pokud ne, vyberte jenom uživatele, který problém nahlásil.</span><span class="sxs-lookup"><span data-stu-id="3024f-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="3024f-112">Pokud **v části Důvod odeslání** vyberete Možnost Měl být zablokován , určete, jestli zpráva měla být zablokovaná jako **Spam**, **Phishing** nebo **Malware,** a pak vyberte **Odeslat.** </span><span class="sxs-lookup"><span data-stu-id="3024f-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="3024f-113">Další informace najdete v článku Jak odeslat do Microsoftu podezřelé [spamy, phish, adresy URL](https://go.microsoft.com/fwlink/?linkid=2101479)a soubory ke skenování .</span><span class="sxs-lookup"><span data-stu-id="3024f-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
