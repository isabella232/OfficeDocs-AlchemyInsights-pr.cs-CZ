---
title: Oprava chyby 0x8004de40 na OneDrivu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745123"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Oprava chyby 0x8004de40 na OneDrivu

Pokud se na OneDrivu zobrazí chyba 0x8004de40:

- Restartujte počítač, který je připojený k doméně adresáře Acitve.
- Pokud se restartováním problém nevyřeší, odpojte se do zařízení z Azure AD a připojte se znovu. 

**Poznámka**: při provádění těchto kroků byste měli být v podnikové síti. Tyto kroky neprovádějte, pokud se nemůžete připojit k podnikové infrastruktuře (například při cestování). 

- Otevřete příkazový řádek se zvýšenými oprávněními. 
- Pokud chcete otevřít příkazový řádek se zvýšenými oprávněními, klikněte na **Start**, pravým tlačítkem myši klikněte na **příkazový řádek**a potom klikněte na **Spustit jako správce**.
- Zadejte *dsregcmd/Leave* a stiskněte **ENTER**.
- Po dokončení zadejte *dsregcmd/JOIN* a stiskněte **ENTER**.
- Po dokončení zavřete příkazový řádek.
- Restartujte počítač a přihlaste se k OneDrivu.