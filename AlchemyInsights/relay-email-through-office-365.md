---
title: Přenos e-mailů přes Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809648"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="2b8eb-102">Nastavení multifunkčního zařízení nebo aplikace na posílání e-mailů</span><span class="sxs-lookup"><span data-stu-id="2b8eb-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="2b8eb-103">Informace o možnostech a postup najdete v článku [Jak nastavit multifunkční zařízení nebo aplikaci na posílání e-mailů pomocí Microsoftu 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="2b8eb-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="2b8eb-104">**Poznámka:** Pokud vám v poslední době přestalo fungovat nějaké zařízení nebo aplikace, připomínáme, že jsme nedávno podle plánu zahájili [vyřazování šifrovacího algoritmu 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="2b8eb-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="2b8eb-105">Pokud se chcete podívat na zařízení, kterých se to týká, přejděte na [Zprávu o ověření klientů SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="2b8eb-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="2b8eb-106">Mohly by se objevit chyby následujících typů: neúspěšné ověření nebo chyba ověření, chyba TLS, chyba šifrovacího algoritmu, neshoda algoritmu nebo přerušené připojení.</span><span class="sxs-lookup"><span data-stu-id="2b8eb-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="2b8eb-107">Řešení problému:</span><span class="sxs-lookup"><span data-stu-id="2b8eb-107">To resolve the issue:</span></span>

 - <span data-ttu-id="2b8eb-108">**Služba Windows Server 2003 IIS SMTP už nebude fungovat – je nutné získat novější verzi Windows.**</span><span class="sxs-lookup"><span data-stu-id="2b8eb-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="2b8eb-109">Ověřte si prosím u dodavatele aplikace nebo zařízení, jestli je podporováno moderní šifrování nebo jestli je k dispozici aktualizace.</span><span class="sxs-lookup"><span data-stu-id="2b8eb-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
