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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062901"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Chyba adresy proxy serveru při vytváření poštovní schránky nebo jiného objektu s povoleným e-mailem

Pokud jste se pokusili vytvořit objekt s podporou e-mailu (poštovní schránka, sdílená poštovní schránka atd.) a dostali jste chybu "Adresa proxy serveru "SMTP:alias@domain.com" se už používá...", je e-mailová adresa, kterou jste vybrali, už pořízená jiným objektem s podporou e-mailu ve vaší organizaci.
  
Musíte najít uživatele, skupinu, sdílenou poštovní schránku nebo veřejnou složku s touto e-mailovou adresou a odstranit ji nebo změnit její e-mailovou adresu. Potom můžete vytvořit nový objekt s podporou e-mailu s bezplatnou e-mailovou adresou. Vyhledejte ho pomocí funkce Hledat na domovské stránce. K jeho vyhledání můžete použít Exchange Online powershellový příkaz:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Pokud stávající e-mailovou adresu nechcete odstranit, zvolte novou e-mailovou adresu pro nový objekt, který vytváříte.
  