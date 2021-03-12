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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Kvůli zákazu TLS 1.0 a TLS 1.1 se nedaří odesílat a přijímat e-maily do/z Office 365

Jak potvrdilo centrum zpráv po mc229914, deprecation TLS 1.0 a TLS 1.1 začalo vynucovat koncové body toku pošty Exchange Online. Brzy už Office 365 nebude přijímat e-mailová připojení TLS 1.0 a TLS 1.1 z externích zdrojů. Exchange Online taky nikdy nebude používat TLS 1.0 nebo 1.1 k odesílání odchozích e-mailů. Pokud máte problémy kvůli zakázání TLS 1.0 nebo 1.1, může dojít k některé z následujících chyb:

- Odesílatel dostává oznámení o nedoručení zpět – '421 4.4.2 Connection dropped due to SocketError'
- Chyba v Prohlížeči front místního serveru, který odesílá e-maily do služby Officer 365– '421 4.4.2 Connection dropped due to SocketError'
- Chyba v protokolu Protokolu pro [odesílání](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) konektorů na serveru odesílajícím e-maily do Office 365 – vyjednávání TLS se nezdařilo s chybou SocketError
- Chyba v protokolu protokolu Odeslat nebo přijmout konektor – '451 5.7.3 Musí nejdřív vydat příkaz STARTTLS.

Pokud dojde k jakékoli z výše uvedených chyb, zkontrolujte prosím, že server, který odesílá nebo přijímá e-maily, má povolený protokol TLS 1.2, a to kontrolou následujících klíčů registru.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Pokud ve výše uvedených klíčích registru změníte povolení tls 1.2, restartujte server, aby se změny projeví. Také se ujistěte, že máte nainstalované nejnovější aktualizace Windows a Exchange.

Další informace najdete tady:

- [Exchange Server tls, část 1: Připravujeme se na TLS 1.2 – technická komunita Microsoftu](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS , část 2: Povolení tls 1.2 a identifikace klientů, kteří ho nepou ít – technická komunita Microsoftu](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Principy scénářů e-mailu v případě, že se verze TLS neschová s Exchangem Online – technická komunita Microsoftu](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
