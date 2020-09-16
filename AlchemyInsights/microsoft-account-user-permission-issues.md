---
title: Řešení problému – uživatel nebyl nalezen v adresáři
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725400"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Řešení problému – uživatel nebyl nalezen v adresáři

Pokud se uživatelům zobrazí chybová zpráva "uživatel nebyl nalezen" v adresáři, zkuste to znovu, kde typ problému uživatel není v adresáři.

Tento problém můžete vyřešit provedením následujících kroků.

- Ujistěte se, že účet, který přijal pozvánku, je stejný účet, který se používá k pozdějšímu přihlášení. Ujistěte se, že uživatel používá stejný účet pro přijetí pozvánky a přihlášení na web. 

Další informace najdete v tématu [jak spravovat aliasy pro váš účet Microsoft </a> pro správu přihlášení Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Přejděte na jednotlivé weby, ve kterých uživatel obdrží chybu. 

Add "/_layouts/15/People.aspx/MembershipGroupId = 0" (uvnitř uvozovek) na konec adresy URL webu. 

Příklad: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Vyberte uživatele ze seznamu.

- Na pásu karet klikněte na **Odebrat uživatelská oprávnění** . 
-  Přidat uživatele a znovu odeslat pozvánku uživateli

