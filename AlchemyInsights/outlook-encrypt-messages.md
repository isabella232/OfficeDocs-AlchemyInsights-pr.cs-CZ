---
title: S/MIME v Outlooku na webu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772255"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="c16e3-102">Šifrování e-mailových zpráv v Outlooku</span><span class="sxs-lookup"><span data-stu-id="c16e3-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="c16e3-103">Šifrování zpráv Microsoft 365 je postavené na platformě Microsoft Azure Rights Management (Azure RMS), která je součástí Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="c16e3-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="c16e3-104">Pokud vaše předplatné obsahuje Azure Rights Management nebo Azure Information Protection, **nemusíte provádět žádné akce pro ruční povolení nebo aktivaci** služby Rights Management.</span><span class="sxs-lookup"><span data-stu-id="c16e3-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="c16e3-105">V závislosti na názorech zákazníků už nebudete moct povolit automatické šifrování odchozích e-mailů s určitým typem citlivých informací ve vašem tenantovi ve výchozím nastavení.</span><span class="sxs-lookup"><span data-stu-id="c16e3-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="c16e3-106">Místo toho nabízíme podrobné pokyny, jak to yourselves.</span><span class="sxs-lookup"><span data-stu-id="c16e3-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="c16e3-107">Další podrobnosti o tom, jak vytvořit pravidlo přenosu pro šifrování citlivých informací, najdete v [tomto článku](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="c16e3-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="c16e3-108">Pokud používáte Outlook na webu (dřív to byl **OWA**): při vytváření e-mailové zprávy jednoduše klikněte na **chránit** v OWA.</span><span class="sxs-lookup"><span data-stu-id="c16e3-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="c16e3-109">Bude použito oprávnění "Nepředávat dál".</span><span class="sxs-lookup"><span data-stu-id="c16e3-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="c16e3-110">Klikněte na **změnit oprávnění** a zvolte **zašifrovat** , abyste zprávu zašifroval jenom.</span><span class="sxs-lookup"><span data-stu-id="c16e3-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="c16e3-111">Pokud používáte **klienta Outlooku**: Pokud chcete poslat šifrovanou zprávu z Outlook 2013 nebo 2016 nebo Outlooku 2016 pro Mac, vyberte **Možnosti**  >  **oprávnění**a pak vyberte požadovanou možnost ochrany.</span><span class="sxs-lookup"><span data-stu-id="c16e3-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="c16e3-112">Chcete **-li automaticky zašifrovat všechny e-maily** poslané určitým příjemcům nebo organizacím externích partnerů, musíte v centru pro správu Exchange vytvořit pravidlo přenosu pošty.</span><span class="sxs-lookup"><span data-stu-id="c16e3-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="c16e3-113">Podrobné pokyny [najdete v tomto článku podpory](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="c16e3-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

