---
title: Konfigurace a rozšíření životnosti tokenů
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916731"
---
# <a name="configure-and-extend-token-lifetimes"></a>Konfigurace a rozšíření životnosti tokenů

Můžete zadat dobu života tokenu Accessu, SAML nebo ID vystaveného společností Microsoft Identity Platform. Životnosti tokenů můžete nastavit pro všechny aplikace ve vaší organizaci, pro víceuživatelské (multi-Organization) aplikaci nebo pro konkrétní instanční objekt ve vaší organizaci. Další informace najdete v článku [Konfigurace životnosti tokenů](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Příklady najdete v [části Příklady konfigurace životnosti tokenů](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Informace o tom, jak nakonfigurovat životnost a kompatibilitu tokenu v Azure Active Directory B2C (Azure AD B2C), najdete v článku [Konfigurace tokenů v Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Článek [Konfigurace chování relace v Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) popisuje metody jednotného přihlašování používané v Azure AD B2C a umožňuje zvolit nejvhodnější metodu jednotného přihlašování při konfiguraci zásad.

**Jak dlouho tokeny vyřešíte? Jak dlouho platí?**

Životnost tokenů je 1 hodina a životnost relace je 24 hodin. To znamená, že pokud se neudělaly žádné žádosti za 24 hodin, budete se muset před žádostí o nový token přihlásit znova.

> [!NOTE]
> Po 30. května 2020 nebude moct žádný nový klient používat konfigurovatelné zásady životnosti tokenů pro konfiguraci a obnovovací tokeny. Odmítání proběhne do několika měsíců od toho, což znamená, že přestáváme dodržovat zásady existujících relací a obnovovacích tokenů. Životnost tokenů přístupu můžete nakonfigurovat po neplatnosti.






