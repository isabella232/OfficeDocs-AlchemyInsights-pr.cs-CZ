---
title: Chyba adresy proxy serveru při vytváření sdílené poštovní schránky
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568283"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Chyba adresy proxy serveru při vytváření poštovní schránky nebo jiného objektu s povoleným e-mailem

Pokud se vám při pokusu o vytvoření objektu s podporou e-mailu (poštovní schránka, sdílená poštovní schránka atd.) zobrazí chybová zpráva "Proxy adresa "SMTP:alias@domain.com" se už používá...", je e-mailová adresa, kterou jste vybrali, už pořízená jiným objektem ve vaší organizaci, který umožňuje e-mail.
  
Musíte najít uživatele, skupinu, sdílenou poštovní schránku nebo veřejnou složku s touto e-mailovou adresou a odstranit ji nebo změnit její e-mailovou adresu. Potom můžete vytvořit nový objekt s povoleným e-mailem a pomocí odemkované e-mailové adresy. K vyhledání použijte pole Hledat na domovské stránce. Můžete ho také vyhledat pomocí následujícího příkazu Exchange Online PowerShellu:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Pokud nechcete odstranit existující e-mailovou adresu, zvolte novou e-mailovou adresu pro nový objekt, který vytváříte.
  