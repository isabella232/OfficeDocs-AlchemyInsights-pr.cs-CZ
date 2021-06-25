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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117976"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="7b96f-102">Nastavení multifunkčního zařízení nebo aplikace na posílání e-mailů</span><span class="sxs-lookup"><span data-stu-id="7b96f-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="7b96f-103">Informace o možnostech a postup najdete v článku [Jak nastavit multifunkční zařízení nebo aplikaci na posílání e-mailů pomocí Microsoftu 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="7b96f-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="7b96f-104">Pokud máte zařízení nebo aplikaci, které nedávno přestaly fungovat, nejčastějšími problémy jsou:</span><span class="sxs-lookup"><span data-stu-id="7b96f-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="7b96f-105">**Chyby související s ověřováním při odesílání klienta SMTP Auth** Nedávno jsme udělali některé změny týkající se toho, jak funguje ověřování SMTP.</span><span class="sxs-lookup"><span data-stu-id="7b96f-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="7b96f-106">Další informace o řešení problémů najdete v části o neúspěšném ověřování v článku Řešení problémů s tiskárnami, skenery a [aplikacemi LOB,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)které odesílaly e-maily pomocí Microsoft 365 nebo Office 365 .</span><span class="sxs-lookup"><span data-stu-id="7b96f-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="7b96f-107">Při vytváření zabezpečeného připojení k síti přijímáme jenom verzi **TLS 1.2 Office 365** Pokud používáte zabezpečené připojení (TLS), ujistěte se, že vaše aplikační zařízení podporuje TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="7b96f-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="7b96f-108">Další informace najdete v tématu [Příprava na TLS 1.2](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)v Office 365 a Office 365 GCC .</span><span class="sxs-lookup"><span data-stu-id="7b96f-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="7b96f-109">Další problémy a řešení najdete v článku Řešení problémů s tiskárnami, skenery a lob aplikacemi, které odesílaly e-maily [Microsoft 365 nebo Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span><span class="sxs-lookup"><span data-stu-id="7b96f-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="7b96f-110">Pokud se chcete podívat na zařízení, kterých se to týká, přejděte na [Zprávu o ověření klientů SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="7b96f-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="7b96f-111">**Poznámka:** Exchange Online scénáře hromadné korespondence.</span><span class="sxs-lookup"><span data-stu-id="7b96f-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="7b96f-112">Pokud chcete posílat hromadné komerční e-maily (například bulletiny zákazníků), měli byste použít poskytovatele třetích stran, kteří se specializují na tyto služby.</span><span class="sxs-lookup"><span data-stu-id="7b96f-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
