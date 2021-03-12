---
title: Kvůli zákazu TLS 1.0 a TLS 1.1 se nedaří odesílat a přijímat e-maily do/z Office 365
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743450"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="ff676-102">Kvůli zákazu TLS 1.0 a TLS 1.1 se nedaří odesílat a přijímat e-maily do/z Office 365</span><span class="sxs-lookup"><span data-stu-id="ff676-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="ff676-103">Jak potvrdilo centrum zpráv po mc229914, deprecation TLS 1.0 a TLS 1.1 začalo vynucovat koncové body toku pošty Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="ff676-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="ff676-104">Brzy už Office 365 nebude přijímat e-mailová připojení TLS 1.0 a TLS 1.1 z externích zdrojů.</span><span class="sxs-lookup"><span data-stu-id="ff676-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="ff676-105">Exchange Online taky nikdy nebude používat TLS 1.0 nebo 1.1 k odesílání odchozích e-mailů.</span><span class="sxs-lookup"><span data-stu-id="ff676-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="ff676-106">Pokud máte problémy kvůli zakázání TLS 1.0 nebo 1.1, může dojít k některé z následujících chyb:</span><span class="sxs-lookup"><span data-stu-id="ff676-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="ff676-107">Odesílatel dostává oznámení o nedoručení zpět – '421 4.4.2 Connection dropped due to SocketError'</span><span class="sxs-lookup"><span data-stu-id="ff676-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="ff676-108">Chyba v Prohlížeči front místního serveru, který odesílá e-maily do služby Officer 365– '421 4.4.2 Connection dropped due to SocketError'</span><span class="sxs-lookup"><span data-stu-id="ff676-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="ff676-109">Chyba v protokolu Protokolu pro [odesílání](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) konektorů na serveru odesílajícím e-maily do Office 365 – vyjednávání TLS se nezdařilo s chybou SocketError</span><span class="sxs-lookup"><span data-stu-id="ff676-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="ff676-110">Chyba v protokolu protokolu Odeslat nebo přijmout konektor – '451 5.7.3 Musí nejdřív vydat příkaz STARTTLS.</span><span class="sxs-lookup"><span data-stu-id="ff676-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="ff676-111">Pokud dojde k jakékoli z výše uvedených chyb, zkontrolujte prosím, že server, který odesílá nebo přijímá e-maily, má povolený protokol TLS 1.2, a to kontrolou následujících klíčů registru.</span><span class="sxs-lookup"><span data-stu-id="ff676-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="ff676-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span><span class="sxs-lookup"><span data-stu-id="ff676-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="ff676-113">Pokud ve výše uvedených klíčích registru změníte povolení tls 1.2, restartujte server, aby se změny projeví.</span><span class="sxs-lookup"><span data-stu-id="ff676-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="ff676-114">Také se ujistěte, že máte nainstalované nejnovější aktualizace Windows a Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff676-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="ff676-115">Další informace najdete tady:</span><span class="sxs-lookup"><span data-stu-id="ff676-115">For more information, see:</span></span>

- [<span data-ttu-id="ff676-116">Exchange Server tls, část 1: Připravujeme se na TLS 1.2 – technická komunita Microsoftu</span><span class="sxs-lookup"><span data-stu-id="ff676-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="ff676-117">Exchange Server TLS , část 2: Povolení tls 1.2 a identifikace klientů, kteří ho nepou ít – technická komunita Microsoftu</span><span class="sxs-lookup"><span data-stu-id="ff676-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="ff676-118">Principy scénářů e-mailu v případě, že se verze TLS neschová s Exchangem Online – technická komunita Microsoftu</span><span class="sxs-lookup"><span data-stu-id="ff676-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
