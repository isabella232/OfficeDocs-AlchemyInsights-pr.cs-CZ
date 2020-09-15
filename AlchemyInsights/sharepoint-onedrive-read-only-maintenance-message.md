---
title: Zpráva o údržbě určená jen pro čtení při pokusu o použití SharePointu nebo OneDrivu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670825"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Zpráva o údržbě určená jen pro čtení při pokusu o použití SharePointu nebo OneDrivu

Při pokusu o použití SharePointu nebo OneDrivu pro některý z následujících scénářů se uživatelům může zobrazit zpráva o **údržbě jen pro čtení** . 

-   Plánovaná nebo aktivní aktivita údržby.  Podívejte se na ně tak, že přejdete do [centra zpráv](https://portal.office.com/adminportal/home#/messagecenter).
-   S vysokou prioritou aktivní servisní události, ke které může dojít. Podívejte se na všechny informační zpravodaje/incidenty – přejděte na [stav služby](https://portal.office.com/adminportal/home#/servicehealth).
-   Nepatrný automatický způsob obnovení, který může nastat kvůli neočekávaným událostem na serverech, které by mohly trvat méně než 30 min. 
    
    U těchto menších obnovení nejsou k dispozici žádná centra zpráv nebo služby stavu služeb, ale měli byste být zpátky na normální.

Na krátkou chvíli jsme narazili na to, že jedna ze tří uvedených scénářů byla příčina, a služba byla obnovena, ale mezipaměť prohlížeče uživatelů nebyla smazána.

Než přejdete na web, zkuste vymazat mezipaměť prohlížeče.

1. V prohlížeči Microsoft Edge vyberte **Nastavení**a pak vyberte **Ochrana osobních údajů a zabezpečení**.
2. V části **Vymazat procházení**vyberte **zvolit, co chcete vymazat**.
3. Vyberte **soubory cookie a data uloženého webu**a vyberte **Vymazat**.

>[!Note] 
> Tento postup se může lišit při používání jiných prohlížečů, jako je Mozilla Firefox nebo Google Chrome.

>[!Note] 
> Další možností je otevřít SharePointový web nebo OneDrive v novém okně InPrivate.