---
title: Oprava problémů s nastavením DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744943"
---
# <a name="fix-dkim-setup-issues"></a>Oprava problémů s nastavením DKIM

Pokud máte problémy s povolením DKIM pro vaši vlastní doménu, postupujte takto:

- Většina problémů s nastavením DKIM souvisí s nesprávnými záznamy DNS. Ověřte, jestli je záznam CNAME DKIM (**ne** záznam TXT) správně naformátovaný. Další informace najdete v tomto [tématu](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Po vytvoření nebo aktualizaci záznamů DNS DKIM u hostitelské služby DNS pro vaši doménu (obvykle u doménového registrátora) Počkejte na rozšíření záznamů DNS.

- Pokud v centru pro správu nemůžete vytvořit záznamy DNS DKIM, můžete je nahradit \<CustomDomain\> vlastní doménou (třeba contoso.com) a spustit tento příkaz v [PowerShellu Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
