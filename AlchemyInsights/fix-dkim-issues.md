---
title: Řešení problémů s nastavením DKIM
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
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945924"
---
# <a name="fix-dkim-setup-issues"></a>Řešení problémů s nastavením DKIM

Pokud máte problémy s povolením funkce DKIM pro vaši vlastní doménu, postupujte takto:

- Většina problémů s nastavením DKIM souvisí s nesprávnými záznamy DNS. Ověřte, jestli je záznam DKIM CNAME **(ne** záznam TXT) naformátovaný správně. Další informace najdete v tomto [tématu](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Po vytvoření nebo aktualizaci záznamů DNS DKIM v hostitelské službě DNS pro vaši doménu (obvykle doménového registrátora) počkejte, až se záznamy DNS rozšíří.

- Pokud nemůžete vytvořit záznamy DNS DKIM v Centru pro správu, můžete nahradit vlastní doménou (například contoso.com) a spustit tento příkaz v \<CustomDomain\> [Exchange Online PowerShellu](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
