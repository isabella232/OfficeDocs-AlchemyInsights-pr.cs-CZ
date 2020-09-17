---
title: Přesunutí e-mailových zpráv do archivní poštovní schránky
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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799773"
---
# <a name="move-email-to-the-archive-mailbox"></a>Přesunutí e-mailu do archivní poštovní schránky

Pokud chcete, abychom mohli spustit automatizované kontroly pro níže uvedené nastavení, klikněte na tlačítko zpět <--v horní části této stránky zadejte e-mailovou adresu uživatele, který má problémy s přesunutím e-mailu do archivované poštovní schránky.

1. Zkontrolujte, že je povolená **poštovní schránka** . Pokud ne, povolte archivaci poštovní schránky podle pokynů v [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) .

2. Pokud chcete, aby se zprávy automaticky archivoval do archivní poštovní schránky, musí být nastavena značka pro uchování informací, která **se má** **automaticky použít u celé značky poštovní schránky (výchozí)**. Postupujte podle pokynů pro vytvoření značky: [výchozí nastavení archivu](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Potom **přidejte do zásad** uchovávání informací. V centru pro správu Exchange zvolte **zásady uchovávání informací** , > přidejte **značku pro přesunutí do** složky > **Uložit**.

4. Teď [přiřaďte zásady uchovávání informací](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) k poštovní schránce určitého uživatele. Stejné zásady se uplatní pro poštovní schránku **hlavní** i **archiv** .

Může být nutné vynutit spuštění pomocníka pro správu složek (MFA) a použít nové nastavení u poštovní schránky uživatele. Spuštěním tohoto příkazu po [připojení k EXO PowerShellu](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) spustíte Pomocníka pro správu složky pro konkrétní poštovní schránku:
  
Start-ManagedFolderAssistant-identita <name of the mailbox>

Další informace o nastavení zásad archivace najdete v tématu [nastavení zásad archivace a odstraňování poštovních schránek](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  