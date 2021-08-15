---
title: Access denied when viewing a Workflow
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955194"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Access denied when viewing a Workflow

SharePoint 2013, které se pokoušejí poslat e-mail skupině SharePoint, selžou s chybovou zprávou "Přístup odepřen", pokud členství ve skupině SharePoint není nastavené na Everyone (Všichni).
  
 **Chcete-li tento problém vyřešit, postupujte takto:**
  
 1. Povolte všem, aby viděli členy SharePoint skupiny.
  
 2. Odeberte skupinu SharePoint z řádku Komu nebo KOPIE e-mailu.
  
 3. Explicitně přidejte uživatele na řádek Komu nebo KOPIE, pokud viditelnost členství pro skupinu SharePoint členství.
  
Další podrobnosti najdete v článku [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  