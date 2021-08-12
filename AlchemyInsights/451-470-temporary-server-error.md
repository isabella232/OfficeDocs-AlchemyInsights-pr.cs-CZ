---
title: 451 4.7.0 Dočasná chyba serveru Zkuste to prosím později. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812575"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Dočasná chyba serveru Zkuste to prosím později. PRX4

Při posílání e-mailů přes smarthost "smtp.office365.com" můžete čelit problému pomocí metody odeslání klienta SMTP a zobrazí se chybová zpráva: "451 4.7.0 Temporary server error. Zkuste to prosím později. PRX4 je většinou dočasný." 

Ujistěte se, že pro odeslání klienta SMTP používáte sdílenou poštovní schránku, protože metoda odeslání klienta SMTP vyžaduje, aby se přes poštu posílala licencovaná poštovní schránka. Pokud ale sdílenou poštovní schránku používáte a problém přetrvává, zkontrolujte následující:

1. Povolte odeslání smtp klienta u licencované poštovní schránky používané spuštěním tohoto příkazu PowerShellu:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    NEBO

    1. Přejděte na Centrum pro správu Microsoftu 365 > **Aktivní uživatelé** a vyberte uživatele.
    1. Přejděte na kartu Pošta a > **e-mailové** > **vyberte Spravovat e-mailové aplikace**. 
    1. Ujistěte **se, že je zaškrtnuté** nastavení Ověřené SMTP (povolené).
    1. Vyberte **Uložit změny**.
    
    Pokud chcete povolit ověřování SMTP pro celou organizaci, spusťte tento příkaz:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Poznámka:** Z bezpečnostních důvodů se doporučuje povolit ověřování SMTP jenom pro poštovní schránku, která se používá. Nastavení na úrovni uživatele přepíše nastavení úrovně organizace.

2. Výchozí nastavení zabezpečení Azure můžete zakázat tak, že **povolíte výchozí nastavení zabezpečení** na **Ne:**

    1. Přihlaste se k webu Azure Portal jako správce zabezpečení, správce podmíněného přístupu nebo globální správce.
    1. Přejděte na Azure Active Directory >**  Vlastnosti a** vyberte **Spravovat výchozí nastavení zabezpečení**.
    1. Nastavte **přepínač Povolit výchozí nastavení** zabezpečení na **Ne**.
    1. Vyberte **Uložit**.

3. Zakažte vícefaktorové ověřování (MFA) u používané licencované poštovní schránky.

    1. Přejděte na Centrum pro správu Microsoftu 365 a v levé navigační nabídce zvolte **Uživatelé**  >  **aktivní uživatelé**.
    1. Na stránce **Aktivní uživatelé** zvolte **Vícefaktorové ověřování**.
    1. Vyberte uživatele a **zakažte vícefaktorové ověřování**.

