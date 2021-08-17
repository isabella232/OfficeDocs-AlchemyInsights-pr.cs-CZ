---
title: Kvůli zákazu TLS 1.0 a TLS 1.1 Office 365 nelze odesílat a přijímat e-maily do/z aplikace
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054899"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Kvůli zákazu TLS 1.0 a TLS 1.1 Office 365 nelze odesílat a přijímat e-maily do/z aplikace

Jak potvrdilo centrum zpráv po zápisu MC229914, deprecation TLS 1.0 a TLS 1.1 začalo vynucovat Exchange Online koncových bodů toku pošty. Brzy Office 365 nebudou přijímat e-mailová připojení TLS 1.0 a TLS 1.1 z externích zdrojů. Také Exchange Online k odesílání odchozích e-mailů nikdy nebude používat TLS 1.0 nebo 1.1. Pokud máte problémy kvůli zakázání TLS 1.0 nebo 1.1, může dojít k některé z následujících chyb:

- Odesílatel dostává oznámení o nedoručení zpět – '421 4.4.2 Connection dropped due to SocketError'
- Chyba v Prohlížeči front místního serveru, který odesílá e-maily do služby Officer 365– '421 4.4.2 Connection dropped due to SocketError'
- Chyba v protokolu Protokolu pro [odesílání](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) konektorů na serveru odesílajícím e-maily Office 365 tls se nepodařilo s chybou SocketError
- Chyba v protokolu protokolu Odeslat nebo přijmout konektor – '451 5.7.3 Musí nejdřív vydat příkaz STARTTLS.

Pokud dojde k jakékoli z výše uvedených chyb, zkontrolujte prosím, že server, který odesílá nebo přijímá e-maily, má povolený protokol TLS 1.2, a to kontrolou následujících klíčů registru.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Pokud ve výše uvedených klíčích registru změníte povolení tls 1.2, restartujte server, aby se změny projeví. Také se ujistěte, že máte nainstalované nejnovější Windows a Exchange aktualizace.

Další informace najdete tady:

- [Exchange Server Pokyny k TLS, část 1: Připravujeme se na TLS 1.2 – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server Pokyny tls, část 2: Povolení TLS 1.2 a identifikace klientů, kteří ho nepou ít – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Principy scénářů e-mailu v případě, že se verze TLS neschová s Exchange Online – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
