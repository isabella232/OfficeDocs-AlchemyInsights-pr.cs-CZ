---
title: Sdílení s externími uživateli nefunguje
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691568"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Řešení problémů se sdílením obsahu služby SharePoint s externími uživateli

Ujistěte se, že je ve vaší organizaci zapnuté externí sdílení:
  
1. Přejděte na [ &amp; stránku doplňky služeb v centru pro správu Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)a klikněte na **weby**.
    
2. Zkontrolujte, jestli je nastavení zapnuté. Pokud je vybraná možnost jenom stávající externí uživatelé, zkontrolujte, jestli je externí uživatel uvedený v centru pro správu Microsoft 365.
    
Zkontrolujte, jestli je na webu zapnuté externí sdílení. Pro klasickou kolekci webů:
  
1. V novém centru pro správu SharePointu v levém podokně klikněte na **weby**.
    
2. Vyberte web nebo weby a na pásu karet klikněte na **sdílení**.
    
Pro týmový web, který patří do skupiny Microsoft 365 nebo komunikační web:
  
- Tyto nové typy webů mají stejné nastavení sdílení jako nastavení pro celou organizaci, pokud toto nastavení neumožňuje sdílení souborů pomocí odkazů, které nevyžadují přihlášení. V tomto případě weby povolí sdílení s novými a stávajícími externími uživateli, kteří se přihlásí. Pokud chcete změnit nastavení pro určité weby, použijte nové centrum pro správu SharePointu nebo PowerShell. [Další informace](https://go.microsoft.com/fwlink/?linkid=871863)
    
> [!NOTE]
> Nastavení externího sdílení libovolného webu může být více omezující než vaše nastavení pro celou organizaci, ale neomezenější než u celé organizace. 
  

