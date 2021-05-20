---
title: 2491 Upozornění na e-mailové zprávy z zásady Phish Delivered due to tenant or user override
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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544571"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="c096a-102">Upozornění na e-mailové zprávy z zásady Phish Delivered (Doručeno z důvodu přepsání tenanta nebo uživatele)</span><span class="sxs-lookup"><span data-stu-id="c096a-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="c096a-103">Pro tenanty s licencí Microsoft Defender pro Office 365 P1 a P2 byla vydaná výchozí zásada upozornění s názvem Phish Delivered z důvodu přepsání tenanta nebo uživatele.</span><span class="sxs-lookup"><span data-stu-id="c096a-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="c096a-104">Pokud jste dostali toto upozornění, tady je postup, jak prozkoumat:</span><span class="sxs-lookup"><span data-stu-id="c096a-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="c096a-105">V upozornění klikněte na **Zobrazit** upozornění a přejděte na stránku **Upozornění** v Centru & dodržování předpisů.</span><span class="sxs-lookup"><span data-stu-id="c096a-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="c096a-106">Výběrem upozornění zobrazíte možnost Zobrazit **seznam zpráv** nebo Zobrazit zprávy **v Průzkumníkovi.**</span><span class="sxs-lookup"><span data-stu-id="c096a-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="c096a-107">Obě tyto možnosti vás převezou k podrobnostem zprávy, která obsahuje ID zprávy.</span><span class="sxs-lookup"><span data-stu-id="c096a-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="c096a-108">Všimněte si, že odkaz Průzkumníka hrozeb automaticky vyfiltruje zprávy, které splňují kritéria upozornění.</span><span class="sxs-lookup"><span data-stu-id="c096a-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="c096a-109">Možná budete muset upravit filtr data v Průzkumníkovi hrozeb.</span><span class="sxs-lookup"><span data-stu-id="c096a-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="c096a-110">Zpráva útoku phishing byla doručena z důvodu ručně nakonfigurovaného přepsání:</span><span class="sxs-lookup"><span data-stu-id="c096a-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="c096a-111">Povolený odesílatel nebo doména nastavená uživatelem</span><span class="sxs-lookup"><span data-stu-id="c096a-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="c096a-112">Povolený odesílatel nebo doména nastavená správcem v zásadách ochrany proti spamu</span><span class="sxs-lookup"><span data-stu-id="c096a-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="c096a-113">Povolená IP adresa v zásadách filtru připojení</span><span class="sxs-lookup"><span data-stu-id="c096a-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="c096a-114">Pravidlo toku pošty (označované taky jako pravidlo přenosu), které je nakonfigurované tak, aby povoloval zprávy.</span><span class="sxs-lookup"><span data-stu-id="c096a-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="c096a-115">Pokud se domníváte, že zpráva byla nesprávně označená jako phish, použijte doplněk Outlook [Report Message](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) (Zpráva sestavy) k odeslání ukázek zpráv do Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="c096a-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
