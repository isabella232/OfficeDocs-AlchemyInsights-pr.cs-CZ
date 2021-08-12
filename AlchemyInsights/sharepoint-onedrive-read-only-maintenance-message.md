---
title: Read-Only k údržbě při pokusu o použití SharePoint nebo OneDrive
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
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910539"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only k údržbě při pokusu o použití SharePoint nebo OneDrive

Při **pokusu** o použití SharePoint nebo OneDrive pro jeden z následujících scénářů se uživatelům může zobrazit zpráva Jen pro čtení pro údržbu. 

-   Plánovaná nebo aktivní údržba.  Zkontrolujte je tak, že přejdete do [Centra zpráv](https://portal.office.com/adminportal/home#/messagecenter).
-   Může dojít k incidentu s vysokou prioritou a aktivní službou. Všechny poradce nebo incidenty můžete zkontrolovat tak, že přejdete na [Stav služby](https://portal.office.com/adminportal/home#/servicehealth).
-   Menší scénář automatického obnovení, ke kterému může dojít v důsledku neočekávaných událostí na serverech, které můžou trvat méně než 30 minut. 
    
    U těchto menších obnovení nejsou žádné příspěvky v Centru zpráv ani Stav služby, ale měli byste se velmi brzy vrátit k normálu.

Při několika málo příležitostech jsme si poznamenali, že příčinou je jeden ze tří výše uvedených scénářů a služba byla obnovena, ale mezipaměť prohlížeče uživatelů nebyla vymazána.

Než přejdete na web, zkuste mezipaměť prohlížeče vymazat.

1. V Microsoft Edge prohlížeči vyberte **Nastavení** a pak vyberte **Ochrana osobních údajů** a zabezpečení .
2. V **části Vymazat procházení** vyberte **Zvolit, co chcete vymazat.**
3. Vyberte **Soubory cookie a uložená data webu** a vyberte **Vymazat**.

>[!Note] 
> Tyto kroky se mohou lišit při používání jiných prohlížečů, jako je Mozilla Firefox nebo Google Chrome.

>[!Note] 
> Další možností by bylo otevřít váš SharePoint nebo OneDrive v novém okně InPrivate.