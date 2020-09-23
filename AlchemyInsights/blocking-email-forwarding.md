---
title: 726 blokování přeposlání e-mailu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219848"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="9e3ae-102">Blokování nebo zrušení blokování přeposílání e-mailů</span><span class="sxs-lookup"><span data-stu-id="9e3ae-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="9e3ae-103">Informace o povolení nebo zakázání předávání [e-](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)mailů pro konkrétní poštovní schránku</span><span class="sxs-lookup"><span data-stu-id="9e3ae-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="9e3ae-104">Na úrovni klienta je kontrola externího předávání provedená pomocí zásad odchozích spamů.</span><span class="sxs-lookup"><span data-stu-id="9e3ae-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="9e3ae-105">Pokud je tato možnost vypnutá nebo automatická, může blokovat přeposílání e-mailů pomocí "550 5.7.520 Access denied, ale vaše organizace neumožňuje chybu externího předávání.</span><span class="sxs-lookup"><span data-stu-id="9e3ae-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="9e3ae-106">V případě, že je předávání nastaveno jako blokované, to je chyba, kterou uživatelé uvidí.</span><span class="sxs-lookup"><span data-stu-id="9e3ae-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="9e3ae-107">Pokud zablokujete přesměrování, ujistěte se, že je zásada nakonfigurovaná tak, aby umožňovala externí přesměrování.</span><span class="sxs-lookup"><span data-stu-id="9e3ae-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="9e3ae-108">Zásady odchozí nevyžádané zprávy můžete zkontrolovat v centru zabezpečení a dodržování předpisů nebo pomocí příkazu Get-HostedOutboundSpamFilterPolicy | FL Name, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="9e3ae-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="9e3ae-109">Pokud chcete nastavit blokování pro přeposílání zpráv, je stejný příkaz shodný se stavem zásad.</span><span class="sxs-lookup"><span data-stu-id="9e3ae-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="9e3ae-110">Poznámka: doporučuje se, aby byl externí Automatický přepočet vypnutý ve výchozích zásadách odchozích Spamních filtrů a povolil se mu jenom pro uživatele, kteří potřebují externí předávání, a to tak, že pro tyto uživatele vytvoří vlastní zásadu.</span><span class="sxs-lookup"><span data-stu-id="9e3ae-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="9e3ae-111">Další informace najdete v článku [konfigurace předávání externích e-mailů v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="9e3ae-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>