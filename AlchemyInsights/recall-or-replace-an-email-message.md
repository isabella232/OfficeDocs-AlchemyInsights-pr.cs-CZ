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
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799197"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Odvolání nebo nahrazení e-mailové zprávy v Microsoft 365

- Můžete **odvolat pouze zprávy, které jsou posílány lidem ve vaší organizaci**. Pokud byla zpráva odeslána na adresu Gmail, například ji nemůžete odvolat.
- **Do počítače můžete odvolat jenom zprávy poslané z outlooku 2016**. Pokud uživatel pošle zprávu pomocí Outlooku pro Mac nebo Outlooku na webu, nemůžete ho odvolat.
- Pokud jste správce, můžete **zprávy odvolat jménem uživatelů pomocí PowerShellu**. V centru pro správu se nedají odvolat zprávy. Další informace najdete v tématu Vyhledání a odstranění e-mailových zpráv v organizaci.

**Odvolání nebo nahrazení odeslané e-mailové zprávy**

1. V podokně složek na levé straně okna Outlooku zvolte složku Odeslaná pošta.
2. Otevřete zprávu, kterou chcete odvolat. Zprávu otevřete poklikáním. Výběr zprávy, aby se zobrazila v podokně čtení, neumožňuje odvolat zprávu.
3. Na kartě zpráva vyberte **Akce**  >  **odvolat zprávu**.
4. Zvolte **Odstranit nepřečtené kopie této zprávy** nebo **Odstranit nepřečtené kopie a nahradit je novou zprávou a**pak vyberte **OK**.
5. Pokud posíláte náhradní zprávu, napište zprávu a pak vyberte **Odeslat**.
6. Úspěšné nebo neúspěšné odvolání zprávy závisí na nastavení příjemců v Outlooku.

Další informace, včetně toho, jak zkontrolovat odvolat, najdete v tématu [odvolání nebo nahrazení e-mailové zprávy, kterou jste odeslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Vyhledání a odstranění e-mailových zpráv v organizaci*** Pokud chcete vyhledat a odstranit e-mailové zprávy ve vaší organizaci, je jednodušší, když jste globální správce. Pokud nejste globální správce, musíte účet přidat do skupiny rolí správce eDiscovery nebo do role pro správu hledání dodržování předpisů. Pokud chcete odstranit zprávy, musíte se připojit ke skupině rolí Správa organizace nebo k roli pro správu vyhledávání a mazání. Oprávnění k těmto rolím se přiřazují v [Centru zabezpečení & dodržování předpisů](https://protection.office.com/).

1. [Vytvořte vyhledávání obsahu](https://docs.microsoft.com/microsoft-365/compliance/content-search) a vyhledejte zprávu, která se má odstranit.
2. [Připojení k PowerShellu centra dodržování předpisů &](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps) 

Pokud používáte VÍCEFAKTOROVÉ ověřování, přečtěte si článek [připojení k systému Microsoft 365 security & centrum dodržování předpisů v PowerShellu pomocí vícefaktorového ověřování](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
