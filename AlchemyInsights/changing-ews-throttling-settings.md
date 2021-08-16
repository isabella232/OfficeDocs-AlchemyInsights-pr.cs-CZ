---
title: Změna nastavení omezení EWS
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968370"
---
# <a name="changing-ews-throttling-settings"></a>Změna nastavení omezení EWS

Spusťte prosím náš automatizovaný test, který vám umožní upravit zásady omezení EWS po dobu trvání migrace. Všimněte si, že i po tomto spuštění budou importy EWS omezeny na 150 MB za 5 minut na poštovní schránku. pokud chcete dosáhnout vyšší propustnosti migrace, migrujte prosím více uživatelů současně.

Upozorňujeme, že změny zásad omezení EWS nemají vliv na následující typy migrace (pomocí nástrojů Microsoftu): Hybridní, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Veřejná složka nebo Služba importu PST.