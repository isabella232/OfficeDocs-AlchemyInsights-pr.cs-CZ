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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693160"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="d7000-102">Odeslání e-mailové zprávy poskytnutím ID síťové zprávy</span><span class="sxs-lookup"><span data-stu-id="d7000-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="d7000-103">V oznámení **o novém odeslání** vyberte **E-mail** a **ID síťové zprávy.**</span><span class="sxs-lookup"><span data-stu-id="d7000-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="d7000-104">ID zprávy pro e-mailovou zprávu v Outlooku najdete takto:</span><span class="sxs-lookup"><span data-stu-id="d7000-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="d7000-105">Poklikejte na e-mailovou zprávu, kterou chcete otevřít.</span><span class="sxs-lookup"><span data-stu-id="d7000-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="d7000-106">Vyberte **vlastnosti**  >  **souboru.**</span><span class="sxs-lookup"><span data-stu-id="d7000-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="d7000-107">Otevřete Poznámkový blok nebo prázdný wordový dokument a pak  zkopírujte a vložte obsah nalezený v internetovém poli záhlaví do otevřeného dokumentu, aby byl líp viditelné.</span><span class="sxs-lookup"><span data-stu-id="d7000-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="d7000-108">Vyhledejte **pole X-MS-Exchange-Organization-Network-Message-Id.**</span><span class="sxs-lookup"><span data-stu-id="d7000-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="d7000-109">Hodnota za : **je** ID, které potřebujete pro odeslání.</span><span class="sxs-lookup"><span data-stu-id="d7000-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="d7000-110">Pokud **se** e-mail příjemcům těchto e-mailů do složky nevyžádané pošty vešla, zvolte **Vybrat vše.**</span><span class="sxs-lookup"><span data-stu-id="d7000-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="d7000-111">Pokud ne, vyberte jenom uživatele, který problém nahlásil.</span><span class="sxs-lookup"><span data-stu-id="d7000-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="d7000-112">Pokud **v části Důvod odeslání** vyberete Možnost Měla být blokována, určete, zda má být zpráva zablokována jako **nevyžádaná** pošta, útok **phishing** nebo **malware,** a pak vyberte **Odeslat.** </span><span class="sxs-lookup"><span data-stu-id="d7000-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="d7000-113">Další informace najdete v článku o odeslání podezřelého [spamu, phishu,](https://go.microsoft.com/fwlink/?linkid=2101479)adres URL a souborů do Microsoftu na skenování.</span><span class="sxs-lookup"><span data-stu-id="d7000-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
