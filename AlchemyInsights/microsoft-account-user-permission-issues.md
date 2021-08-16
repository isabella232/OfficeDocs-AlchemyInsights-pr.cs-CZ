---
title: Poradce při potížích – Uživatel nebyl nalezen v adresáři
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098163"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Poradce při potížích – Uživatel nebyl nalezen v adresáři

Pokud se uživatelům v adresáři zobrazí chybová zpráva "uživatel nemůže být nalezen", zkuste to prosím znovu tam, kde je typ problému Uživatel není v adresáři.

Pokud chcete problém vyřešit, můžete provést následující kroky.

- Ujistěte se, že účet, který přijal e-mailovou pozvánku, je stejný účet, který se používá k pozdějšímu přihlášení. Ujistěte se, že uživatel používá stejný účet k přijetí pozvánky a přihlášení k webu. 

Další informace najdete v tématu Správa aliasů pro váš účet Microsoft pro [ </a> správu přihlašovacích Microsoft 365 účtu.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Přejděte na jednotlivé weby, na kterých se uživateli chyba zobrazí. 

Přidejte "/_layouts/15/people.aspx/membershipgroupid=0" (v uvozovkách) na konec adresy URL webu. 

Příklad: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- V seznamu vyberte uživatele.

- Na **pásu karet klikněte** na Odebrat uživatelská oprávnění. 
-  Přidejte zpět uživatele a znovu odeslat pozvánku uživateli.

