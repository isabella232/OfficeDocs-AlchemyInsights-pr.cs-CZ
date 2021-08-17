---
title: Povolení ověřování SMTP a odstraňování potíží
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
- "3000003"
- "5652"
ms.openlocfilehash: d16389ca577970deaf743255f75dc86134e79dcab2fff8c33987532fc7ee1105
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890427"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Povolení ověřování SMTP a odstraňování potíží

Pokud chcete povolit ověřování SMTP pro poštovní schránku nebo se vám zobrazí chyba "Klient není ověřen", "Ověřování neúspěšné" nebo "SmtpClientAuthentication" s kódem 5.7.57 nebo 5.7.3 nebo 5.7.139 při pokusu o přenos e-mailů ověřením zařízení nebo aplikace s Microsoft 365, proveďte tyto tři akce k vyřešení problému:

1. Výchozí nastavení [zabezpečení Azure můžete zakázat](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) tak, že **povolíte výchozí nastavení zabezpečení** na **Ne**.

    a. Přihlaste se k webu Azure Portal jako správce zabezpečení, správce podmíněného přístupu nebo globální správce.<BR/>
    b. Přejděte na Azure Active Directory > **vlastnosti**.<BR/>
    c. Vyberte **Spravovat výchozí nastavení zabezpečení**.<BR/>
    d. Nastavte **povolit výchozí nastavení zabezpečení na** **Ne**.<BR/>
    e. Vyberte **Uložit**.

2. [Povolte odeslání smtp klienta](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) u licencované poštovní schránky.

    a. V Centrum pro správu Microsoftu 365 přejděte na **Aktivní uživatelé** a vyberte uživatele.<BR/>
    b. Přejděte na kartu Pošta a v části **E-mailové aplikace** vyberte **Spravovat e-mailové aplikace**.<BR/>
    d. Ujistěte **se, že je zaškrtnuté** políčko Ověřený protokol SMTP (povoleno).<BR/>
    e. Vyberte **Uložit změny**.<BR/>

3. [V licencované poštovní schránce zakažte](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) vícefaktorové ověřování (MFA).

    a. Přejděte na Centrum pro správu Microsoftu 365 a v levé navigační nabídce vyberte **Uživatelé**  >  **aktivní uživatelé**.<BR/>
    b. Vyberte **Vícefaktorové ověřování**.<BR/>
    c. Vyberte uživatele a **zakažte vícefaktorové ověřování**.<BR/>
