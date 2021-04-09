---
title: Oprava 0x8004de40 v OneDrivu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649741"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Oprava 0x8004de40 v OneDrivu

Pokud používáte Windows 7 a zobrazí se tato chyba, aktualizujte protokol [TLS 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)jako výchozí zabezpečené protokoly ve WinHTTP ve Windows .

Pokud používáte Windows 10 a na OneDrivu se zobrazí 0x8004de40 chyba:

- Restartujte ovlivněný počítač při připojení k doméně adresáře Acitve.
- Pokud restartování problém nevyřeší, odpojte se a znovu se ke svému zařízení připojíte z Azure AD. 

**Poznámka:** Při provádění těchto kroků byste měli být v podnikové síti. Tyto kroky nedělejte, když nejste připojení ke své podnikové infrastruktuře (například na cestách). 

1. Otevřete příkazový řádek se zvýšenými oprávněními tak, že **vyberete Start,** klikněte pravým tlačítkem myši na **Příkazový řádek** a pak vyberte **Spustit jako správce.**

1. Zadejte *dsregcmd /leave a* stiskněte **Enter.**

1. Po dokončení zadejte *dsregcmd /join* a stiskněte **Enter.**

1. Po dokončení zavřete příkazový řádek.

1. Restartujte počítač a přihlaste se k OneDrivu.