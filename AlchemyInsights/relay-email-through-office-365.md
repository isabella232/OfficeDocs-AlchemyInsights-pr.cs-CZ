---
title: Přenos e-mailů přes Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 074a9106553bf3a2a5e563f9ebaca9dfc38111cb
ms.sourcegitcommit: 9872280f71429d2344b0b441e218fba5b3bd3cf7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/02/2020
ms.locfileid: "45023452"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="eda5e-102">Nastavení multifunkčního zařízení nebo aplikace na posílání e-mailů</span><span class="sxs-lookup"><span data-stu-id="eda5e-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="eda5e-103">Informace o možnostech a postup najdete v článku [Jak nastavit multifunkční zařízení nebo aplikaci na posílání e-mailů pomocí Microsoftu 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="eda5e-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="eda5e-104">**Poznámka:** Pokud vám v poslední době přestalo fungovat nějaké zařízení nebo aplikace, připomínáme, že jsme nedávno podle plánu zahájili [vyřazování šifrovacího algoritmu 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="eda5e-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="eda5e-105">Pokud se chcete podívat na zařízení, kterých se to týká, přejděte na [Zprávu o ověření klientů SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="eda5e-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="eda5e-106">Mohly by se objevit chyby následujících typů: neúspěšné ověření nebo chyba ověření, chyba TLS, chyba šifrovacího algoritmu, neshoda algoritmu nebo přerušené připojení.</span><span class="sxs-lookup"><span data-stu-id="eda5e-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="eda5e-107">Řešení problému:</span><span class="sxs-lookup"><span data-stu-id="eda5e-107">To resolve the issue:</span></span>

 - <span data-ttu-id="eda5e-108">**Služba Windows Server 2003 IIS SMTP už nebude fungovat – je nutné získat novější verzi Windows.**</span><span class="sxs-lookup"><span data-stu-id="eda5e-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="eda5e-109">Ověřte si prosím u dodavatele aplikace nebo zařízení, jestli je podporováno moderní šifrování nebo jestli je k dispozici aktualizace.</span><span class="sxs-lookup"><span data-stu-id="eda5e-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
