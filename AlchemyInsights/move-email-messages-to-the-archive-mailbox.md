---
title: Přesunutí e-mailových zpráv do poštovní schránky archivu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974950"
---
# <a name="move-email-to-the-archive-mailbox"></a>Přesunutí e-mailu do archivační poštovní schránky

Pokud chcete, abychom pro níže uvedená nastavení spouštěli automatické kontroly, vyberte tlačítko Zpět <– v horní části této stránky a potom zadejte e-mailovou adresu uživatele, který má problémy s přesouváním e-mailů do archivační poštovní schránky.

1. Ověřte, že **je povolená** poštovní schránka archivu. Pokud ne, povolte [archivační](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) poštovní schránku podle pokynů v tomto článku.

2. Pokud chcete archivovat zprávy automaticky do archivační poštovní schránky, musí být značka uchovávání informací s akcí Přesunout do archivu nastavená tak, aby se automaticky použila na celou **značku poštovní schránky (výchozí).**  Pomocí tohoto postupu vytvořte značku: [Archivovat výchozí značku](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Potom přidejte **značku Archiv** do zásad uchovávání informací. V centru Exchange správy **zvolte** Zásady uchovávání informací a > přidat značku **Přesunout** do archivu do zásady > **Uložit.**

4. Teď [přiřaďte zásady uchovávání](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) informací poštovní schránce konkrétního uživatele. Stejná zásada se použije pro  primární i **archivační poštovní schránku.**

Může být nutné vynutit, aby pomocník pro spravované složky spouštěl nové nastavení poštovní schránky uživatele. Spuštěním následujícího příkazu při [připojení k EXO PowerShellu](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) spusťte Pomocníka pro spravované složky pro konkrétní poštovní schránku:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Další informace o nastavení zásad archivace najdete v tématu Nastavení zásad archivace a odstranění [poštovních schránek](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  