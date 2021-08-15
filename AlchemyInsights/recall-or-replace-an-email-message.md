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
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024379"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Odvolání nebo nahrazení e-mailové zprávy v Microsoft 365

- Odvolat můžete jenom zprávy odeslané lidem **ve vaší organizaci**. Pokud byla například zpráva odeslána na adresu Gmailu, nemůžete ji odvolat.
- Zprávy odeslané z počítače Outlook **odvolat.** Pokud uživatel odešle zprávu pomocí Outlook pro Mac nebo Outlook na webu, nemůžete ji odvolat.
- Jako správce tenanta můžete odvolat zprávy jménem uživatelů pomocí **PowerShellu** (Další informace najdete v tématu Vyhledání a [odstranění e-mailových zpráv](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Nemůžete odvolat zprávy z Centra pro správu. Další informace najdete v části Vyhledání a odstranění e-mailových zpráv ve vaší organizaci.

**Odvolání nebo nahrazení odeslané e-mailové zprávy**

1. V podokně složek v levé části okna Outlook vyberte složku Odeslaná pošta.
2. Otevřete zprávu, kterou chcete odvolat. Zprávu otevřete poklikaní. Když vyberete zprávu tak, aby se zobrazí v podokně čtení, nebude možné zprávu odvolat.
3. Na kartě Zpráva vyberte Akce  >  **Odvolat tuto zprávu**.
4. Zvolte **Odstranit nepřečtené kopie** této zprávy nebo Odstranit nepřečtené kopie a nahraďte ji novou **zprávou a** pak vyberte **OK.**
5. Pokud posíláte náhradní zprávu, vytvořte zprávu a pak vyberte **Odeslat.**
6. Úspěch nebo neúspěch odvolání zprávy závisí na nastavení příjemců v Outlook.

Další informace, včetně toho, jak zkontrolovat odvolání, najdete v tématu Odvolání nebo nahrazení odeslané [e-mailové zprávy.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Pokud chcete hledat a odstraňovat e-mailové zprávy*** ve vaší organizaci , je nejjednodušší, když jste globální správce. Pokud nejste globální správce, musí být váš účet přidán do skupiny rolí Správce eDiscovery nebo do role správy hledání dodržování předpisů. Pokud chcete odstranit zprávy, musíte se připojit ke skupině rolí Správa organizace nebo k roli správy Hledání a čištění. Oprávnění k těmto rolím jsou přiřazena v [Centru & dodržování předpisů](https://protection.office.com/).

1. [Vytvořte hledání obsahu a](https://docs.microsoft.com/microsoft-365/compliance/content-search) vyhledejte zprávu, kterou chcete odstranit.
2. [Připojení na Centrum & dodržování předpisů PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Pokud používáte MFA (vícefaktorové ověřování), podívejte se Připojení na [Microsoft 365 Security & Compliance Center PowerShellu pomocí vícefaktorového ověřování.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
