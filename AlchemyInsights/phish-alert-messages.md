---
title: e-mailové zprávy s výstrahou 2491 z zásady "phishing dodáno" v důsledku zásad přepsání tenanta nebo uživatele
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728604"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="9ed0b-102">Upozorňovat e-mailové zprávy z "funkce phishing dodaná z důvodu zásad přepsání tenanta nebo uživatele"</span><span class="sxs-lookup"><span data-stu-id="9ed0b-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="9ed0b-103">Výchozí zásada upozornění s názvem "phishing Doručená z důvodu přepisu tenanta nebo uživatele" byla zahrnuta do tenanta prostřednictvím licencí Office 365 ATP.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="9ed0b-104">Pokud jste dostali toto upozornění, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="9ed0b-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="9ed0b-105">Kliknutím na **Zobrazit** upozornění v okně upozornění přejděte na stránku **Upozornění** v centru zabezpečení &.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="9ed0b-106">Výběrem výstrahy zobrazíte možnost **Zobrazit seznam zpráv** nebo **Zobrazit zprávy v Průzkumníkovi**.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="9ed0b-107">V obou těchto možnostech se zobrazí podrobnosti zprávy, která obsahuje ID zprávy.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="9ed0b-108">Uvědomte si, že odkaz v Průzkumníku hrozeb automaticky filtruje zprávy, které splňují kritéria upozornění.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="9ed0b-109">Možná bude potřeba upravit filtr data v Průzkumníku hrozeb.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="9ed0b-110">Zpráva útoku phishing byla doručena z důvodu ručně konfigurovaného přepsání:</span><span class="sxs-lookup"><span data-stu-id="9ed0b-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="9ed0b-111">Povoleného odesílatele nebo domény nastavené uživatelem.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="9ed0b-112">Povolený odesílatel nebo doména nastavená správcem v zásadách ochrany proti nevyžádané poště.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="9ed0b-113">Povolená IP adresa v zásadách filtru připojení.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="9ed0b-114">Pravidlo toku pošty (známé taky jako pravidlo přenosu), které je nakonfigurované tak, aby umožňovalo zprávy ve službě.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="9ed0b-115">Pokud se domníváte, že zpráva byla nesprávně označená jako phishing, [použijte k odeslání](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) ukázek zpráv do Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
