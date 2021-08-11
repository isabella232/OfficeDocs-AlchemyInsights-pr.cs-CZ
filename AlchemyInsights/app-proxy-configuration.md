---
title: Konfigurace proxy serveru aplikace
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951558"
---
# <a name="app-proxy-configuration"></a>Konfigurace proxy serveru aplikace

1. Pokud chcete pochopit, jak nakonfigurovat aplikaci Proxy aplikací v Azure AD tak, aby vystavěly vaše místní aplikace do cloudu, podívejte se na postup konfigurace aplikace [Proxy aplikací](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Jednotné přihlašování (SSO) umožňuje uživatelům přístup k aplikaci bez opakovaného ověřování. Umožňuje jednotné ověřování v cloudu, proti Azure Active Directory a umožňuje službě nebo konektoru, aby se zosobňoval uživateli, aby mohl z aplikace provést další problémy s ověřováním. Další informace najdete v tématu Konfigurace jednotného [přihlašování k aplikaci Proxy aplikace](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Tento [článek se používá](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) k řešení běžných problémů, se které lidé řešou při vytváření nové proxy aplikace.
4. Pokud máte potíže s nastavením back-end ověřování aplikace, budete možná muset vyřešit omezené konfigurace delegování protokolu [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) pro Proxy aplikace nebo postupujte podle pokynů ke konfiguraci aplikace pomocí [funkce PingAccess,](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) abyste vyřešili váš problém.
