---
title: Odvolání nebo nahrazení e-mailové zprávy
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353499"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Odvolání nebo nahrazení e-mailové zprávy v Microsoft 365

- Můžete **odvolat pouze zprávy, které jsou posílány lidem ve vaší organizaci**. Pokud je třeba zpráva odeslána na adresu Gmail, nemůžete ji odvolat.
- **Do počítače můžete odvolat pouze zprávy poslané z Outlooku**. Pokud uživatel pošle zprávu pomocí Outlooku pro Mac nebo Outlooku na webu, nemůžete ho odvolat.
- Jako správce klienta můžete **zprávy odvolat jménem uživatelů pomocí PowerShellu** (Další informace najdete v tématu [hledání a odstranění e-mailových zpráv](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- V centru pro správu se nedají odvolat zprávy. Další informace najdete v tématu Vyhledání a odstranění e-mailových zpráv v organizaci.

**Odvolání nebo nahrazení odeslané e-mailové zprávy**

1. V podokně složek na levé straně okna Outlooku zvolte složku Odeslaná pošta.
2. Otevřete zprávu, kterou chcete odvolat. Zprávu otevřete poklikáním. Výběr zprávy, aby se zobrazila v podokně čtení, neumožňuje odvolat zprávu.
3. Na kartě zpráva vyberte **Akce**  >  **odvolat zprávu**.
4. Zvolte **Odstranit nepřečtené kopie této zprávy** nebo **Odstranit nepřečtené kopie a nahradit je novou zprávou a** pak vyberte **OK**.
5. Pokud posíláte náhradní zprávu, napište zprávu a pak vyberte **Odeslat**.
6. Úspěšné nebo neúspěšné odvolání zprávy závisí na nastavení příjemců v Outlooku.

Další informace, včetně toho, jak zkontrolovat odvolat, najdete v tématu [odvolání nebo nahrazení e-mailové zprávy, kterou jste odeslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Pokud chcete **_Vyhledat a odstranit e-mailové zprávy ve vaší organizaci_**, je jednodušší, když jste globální správce. Pokud nejste globální správce, musíte účet přidat do skupiny rolí správce eDiscovery nebo do role pro správu hledání dodržování předpisů. Pokud chcete odstranit zprávy, musíte se připojit ke skupině rolí Správa organizace nebo k roli pro správu vyhledávání a mazání. Oprávnění k těmto rolím se přiřazují v [Centru zabezpečení & dodržování předpisů](https://protection.office.com/).

1. [Vytvořte vyhledávání obsahu](https://docs.microsoft.com/microsoft-365/compliance/content-search) a vyhledejte zprávu, která se má odstranit.
2. [Připojení k PowerShellu centra dodržování předpisů &](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

Pokud používáte VÍCEFAKTOROVÉ ověřování (Multi-Factor Authentication), najdete další informace v tématu [připojení k webu Centrum pro kompatibilitu se systémem & 365 pomocí vícefaktorového ověřování](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
