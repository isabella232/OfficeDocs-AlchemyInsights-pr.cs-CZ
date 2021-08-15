---
title: Konfigurace služby Zřizování
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
- "9004687"
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033271"
---
# <a name="configuring-the-provision-service"></a>Konfigurace služby Zřizování

Aby automatické zřizování uživatelů fungovalo, vyžaduje Azure AD platné přihlašovací údaje, které mu umožní připojit se k rozhraní Workday Web Services API. Tlačítko Testovat připojení v aplikaci Workday to AD User Provisioning také ověřuje, jestli se může připojit k agentu zřizování Azure AD Připojení přidruženému k doméně AD.

Pokud portál Azure Portal vrací chybu při ukládání přihlašovacích údajů, postupujte podle následujících doporučených kroků:

1. Ověřte, že jste nakonfigurovali uživatelský účet systému integrace pracovního dne, jak je uvedeno v části kurzu Konfigurace uživatele systému integrace [v aplikaci Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Ověřte, že služba Azure AD Připojení Provisioning Agent Service je spuštěná na místním Windows serveru pomocí Konzoly pro správu služeb. Stav agenta můžete taky zkontrolovat na portálu Azure portal kliknutím na tlačítko Zobrazit místní agenty.
3. Ujistěte se, že zadáte hodnotu pole "Uživatelské jméno pracovního dne" pomocí formátu username@workday-tenant-name. Pokud název pracovního dne-tenanta chybí, ověřování Workday se nezdaří.
4. Pokud konfigurujete integraci s tenantem implementace Workday, poznamenejte si plánovanou dobu prostojů vašeho tenanta Workday. Pracovní den naplánuje pro tenanty implementace přes víkendy (obvykle od pátečního večera do sobotního dopoledne) a selhání připojení během tohoto prostoje je známý problém, který se automaticky vyřeší, jakmile budou implementační tenanti zase online.
5. Ve výjimečných případech se tato chyba může zobrazit i v případě, že se heslo uživatele systému integrace změnilo kvůli aktualizaci tenanta nebo pokud je účet uzamčený nebo vypršela jeho platnost. Zkontrolujte prosím stav uživatele systému integrace u správce Workday.

Další podrobnosti o konfiguraci pracovního dne pro automatické zřizování najdete v tématu [Kurz:](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)Konfigurace pracovního dne pro automatické zřizování uživatelů .
