---
title: Outlook Odvolání nebo nahrazení e-mailové zprávy na ploše
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918388"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Odvolání nebo nahrazení Outlook e-mailové zprávy

- Jako správce můžete odvolat zprávy jménem uživatelů **používajících PowerShell.** Nemůžete odvolat zprávy z Centra pro správu.
- Odvolat můžete jenom zprávy odeslané lidem **ve vaší organizaci**. Pokud byla zpráva odeslána například na adresu Gmailu, nemůžete ji odvolat.
- Zprávy odeslané z počítače Outlook 2016 **odvolat.** Pokud uživatel odešle zprávu pomocí Outlook pro Mac nebo Outlook na webu, nemůžete ji odvolat.

Odvolání nebo nahrazení e-mailové zprávy:

1. V podokně složek v levé části okna Outlook vyberte složku Odeslaná pošta.
1. Poklikejte na zprávu, kterou chcete odvolat, a otevřete ji.
1. Vyberte kartu **Zpráva** a pak vyberte **Akce Odvolat** tuto  >  **zprávu**.
1. Vyberte **Odstranit nepřečtené** kopie této zprávy nebo Odstranit nepřečtené kopie a nahradit novou **zprávou a** pak vyberte **OK.**
1. Pokud posíláte náhradní zprávu, vytvořte zprávu a pak vyberte **Odeslat.**
1. Úspěch nebo neúspěch odvolání zprávy závisí na nastavení příjemce v Outlook. Postup pro kontrolu odvolání najdete v [tomto článku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Hledání a odstraňování e-mailových zpráv ve vaší organizaci

- Pokud nejste globální správce, musí být váš účet přidaný do role Správce eDiscovery nebo do role správy hledání dodržování předpisů, aby se hledaly zprávy. Pokud chcete odstranit zprávy, musíte se připojit ke skupině rolí Správa organizace nebo k roli správy Hledání a čištění. Oprávnění pro tyto role jsou přiřazena v Centru zabezpečení a [dodržování předpisů](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Vytvořte hledání obsahu a](https://docs.microsoft.com/microsoft-365/compliance/content-search) vyhledejte zprávu, kterou chcete odstranit.
- Připojení do Centra zabezpečení a [dodržování předpisů PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Pokud používáte vícefaktorové ověřování, podívejte se Připojení na Microsoft 365 a Centrum dodržování předpisů [PowerShellu pomocí vícefaktorového ověřování](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).