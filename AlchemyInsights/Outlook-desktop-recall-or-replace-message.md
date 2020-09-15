---
title: Stažení nebo nahrazení e-mailové zprávy v Outlooku
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
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663983"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Odvolání nebo nahrazení e-mailové zprávy Outlooku

- Jako správce můžete **zprávy odvolat jménem uživatelů pomocí PowerShellu**. V centru pro správu se nedají odvolat zprávy.
- Můžete **odvolat pouze zprávy, které jsou posílány lidem ve vaší organizaci**. Pokud byla zpráva odeslána na adresu Gmail, například ji nemůžete odvolat.
- **Do počítače můžete odvolat pouze zprávy odeslané z outlooku 2016**. Pokud uživatel pošle zprávu pomocí Outlooku pro Mac nebo Outlooku na webu, nemůžete ho odvolat.

Odvolání nebo nahrazení e-mailové zprávy:

1. V podokně složek na levé straně okna Outlooku vyberte složku Odeslaná pošta.
1. Poklikejte na zprávu, kterou chcete odvolat, a otevřete ji.
1. Vyberte kartu **zpráva** a pak vyberte **Akce**Odvolejte  >  **tuto zprávu**.
1. Vyberte **Odstranit nepřečtené kopie této zprávy** nebo **Odstranit nepřečtené kopie a nahradit je novou zprávou**a pak vyberte **OK**.
1. Pokud posíláte náhradní zprávu, napište zprávu a pak vyberte **Odeslat**.
1. Úspěšné nebo neúspěšné odvolání zprávy závisí na nastaveních příjemce v Outlooku. Postup pro kontrolu odvolání najdete v [tomto článku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Vyhledání a odstranění e-mailových zpráv v organizaci

- Pokud nejste globálním správcem, musí být váš účet přidán do role správce eDiscovery nebo role pro správu vyhledávání dodržování předpisů pro hledání zpráv. Pokud chcete odstranit zprávy, musíte se připojit ke skupině rolí Správa organizace nebo k roli pro správu vyhledávání a mazání. Oprávnění pro tyto role jsou přiřazena v [Centru zabezpečení a dodržování předpisů](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Vytvořte vyhledávání obsahu](https://docs.microsoft.com/microsoft-365/compliance/content-search) a vyhledejte zprávu, která se má odstranit.
- [Připojení k PowerShellu pro zabezpečení a dodržování předpisů](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Pokud používáte vícefaktorové ověřování, přečtěte si článek [připojení k prostředí PowerShell pro zabezpečení a dodržování předpisů pro systém Microsoft 365 pomocí vícefaktorového ověřování](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).