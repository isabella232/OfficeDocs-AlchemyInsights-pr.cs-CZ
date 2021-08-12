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
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910359"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Řešení problémů se sdílením SharePoint s externími uživateli

Zkontrolujte, jestli je pro vaši organizaci zapnuté externí sdílení:
  
1. Přejděte na [stránku Doplňky služeb &amp; v](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)Centrum pro správu Microsoftu 365 a klikněte na **Weby.**
    
2. Ujistěte se, že je nastavení zapnuté. Pokud je vybraná možnost Pouze existující externí uživatelé, zkontrolujte, jestli je externí uživatel uvedený v Centrum pro správu Microsoftu 365.
    
Ujistěte se, že je externí sdílení pro web zapnuté. Pro klasickou kolekci webů:
  
1. V novém SharePoint pro správu klikněte v levém podokně na **Weby**.
    
2. Vyberte web nebo weby a na pásu karet klikněte na **Sdílení.**
    
Pro týmový web, který patří do Microsoft 365 skupiny nebo komunikačního webu:
  
- Tyto nové typy webů mají stejné nastavení sdílení jako nastavení pro celou organizaci, pokud nastavení pro celou organizaci nepomáhá sdílení souborů pomocí odkazů, které nevyžadují přihlášení. V takovém případě weby umožňují sdílení s novými a stávajícími externími uživateli, kteří se přihlašují. Pokud chcete změnit nastavení pro konkrétní weby, použijte nové centrum pro SharePoint nebo PowerShell. [Další informace](https://go.microsoft.com/fwlink/?linkid=871863)
    
> [!NOTE]
> Nastavení externího sdílení pro libovolný web může být restriktivní než nastavení pro celou organizaci, ale ne více schůdné než nastavení pro celou organizaci. 
  

