---
title: Konfigurace služby zřizování
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
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481343"
---
# <a name="configuring-the-provision-service"></a>Konfigurace služby zřizování

Aby automatické zřizování uživatelů fungovalo, vyžaduje Azure AD platné přihlašovací údaje, které mu umožňují připojení k rozhraní API webových služeb Workday. Tlačítko Test připojení v pracovním dni dále ověřuje i aplikaci ad User Provisioning, jestli se může připojit k agentovi zřizování Azure AD Connect přidruženému k doméně služby AD.

Pokud portál Azure Portal při ukládání přihlašovacích údajů vrací chybu, postupujte podle doporučených kroků níže:

1. Potvrďte, že jste nakonfigurovali uživatelský účet systému Workday Integration System, jak je uvedeno v oddílu Konfigurace uživatele systému integrace [v pracovním dni.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Potvrďte, že služba Azure AD Connect Provisioning Agent (Agent Azure AD) je spuštěná na vašem místním serveru Windows pomocí konzoly pro správu služeb. Stav agenta můžete zkontrolovat i na portálu Azure Portal kliknutím na tlačítko Zobrazit místní agenty.
3. Ujistěte se, že zadáváte hodnotu do pole Workday Username pomocí formátu username@workday-název tenanta. Pokud chybí název pracovního dne-tenanta, ověření pracovního dne selže.
4. Pokud konfigurujete integraci s tenantem implementace Workday, poznamenejte si naplánovanou pracovní dobu tenanta. Pracovní den naplánovat pro tenanty implementace přes víkendy (obvykle od pátečního večera do soboty ráno) a selhání připojení během tohoto intervalu prostoje je známý problém, který se automaticky vyřeší, jakmile tenanti pro implementaci budou zase online.
5. Ve výjimečných případech se tato chyba může zobrazit také v případě, že se změnilo heslo uživatele systému integrace kvůli aktualizaci tenanta nebo když je účet uzamčený nebo jeho platnost vypršela. Zkontrolujte prosím stav uživatele systému integrace s vaším správcem pracovního dne.

Další podrobnosti o konfiguraci pracovního dne pro automatické zřizování najdete v kurzu: Konfigurace [funkce Workday pro automatické zřizování uživatelů.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
