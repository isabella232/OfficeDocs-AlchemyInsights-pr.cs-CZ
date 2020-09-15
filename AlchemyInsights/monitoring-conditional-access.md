---
title: Sledování podmíněného přístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702896"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Sledování podmíněného přístupu pro Exchange

Uživatelé s podmíněným přístupem budou dostávat e-mailové zprávy, pokud nesplňují požadavky na přístup vaší organizace. Chcete-li vyřešit problém, doporučujeme jedno nebo více následujících řešení:
  
- Pokud se předpokládá, že je zařízení zaregistrované, poraďte se s tím, že přejde do aplikace Portál společnosti a ověří, že se zobrazí na portálu společnosti. Pokud to nepomůže, uživatel by měl zařízení zaregistrovat.
    
- Na portálu Azure Portal přejděte na ** \> kompatibilitu zařízení**. V části **monitor** klikněte na položku **dodržování předpisů**. Zobrazte sestavu dodržování předpisů zařízení a ověřte, že zařízení uživatele je označené jako kompatibilní. 
    
- Na portálu Azure Portal přejděte na ** \> kompatibilitu zařízení**. V části **Spravovat**klikněte na **zásady**. V seznamu zásad dodržování předpisů ověřte, zda je k zařízení uživatele přiřazen profil. Pokud není přiřazen žádný profil, nebude moci Intune potvrdit jeho stav. 
    
- Upravte přiřazení podmíněného přístupu uživatele.
    
1. V Azure Portalu přejděte na ** \> \> zásady podmíněného přístupu** .
    
2. V seznamu vyberte zásadu
    
3. Klikněte na **Uživatelé a skupiny** .
    
4. Chcete-li určit určitou zásadu, přidejte ji do seznamu **zahrnutí** . Chcete-li zajistit, aby některá osoba byla ze zásady vynechána, přidejte ji do seznamu **vyloučení** . 
    
Další informace: [sledování zařízení podmíněného přístupu](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

