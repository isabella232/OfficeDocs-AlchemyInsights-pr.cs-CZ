---
title: 1065 neEOP odchozí IP adresy rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806788"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>NeEOPování odchozích rozsahů IP adres

Zjistili jsme potenciální problém ve vaší organizaci, který (Pokud není opraven 26th) 2018, může přerušit tok pošty do místních nebo externích cílů. Pokud chcete správu rozsahu IP adres zjednodušit, slučujeme rozsahy IP adres ochrany Exchange Online (EOP), které se používají k posílání a přijímání e-mailů mimo Microsoft 365. Naše analýza naznačuje, že jeden nebo více externích zdrojů nebo cílů, které jste nakonfigurovali ve spojnicích toku pošty, nepřijímá připojení ze [zde](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)uvedených rozsahů IP adres.

Zajistěte, aby tyto zdroje a cíle přijímaly připojení ke všem [publikovaným EOP adresám](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)a 26th.

Další informace o této změně naleznete v centru zpráv příspěvky [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)nebo [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Poznámka**: Pokud jste v rámci aktualizací koncového bodu používali funkci publikování na adresy IP, XML a RSS, měli byste také migrovat do nových webových služeb pro automatizaci těchto typů aktualizací. Další informace najdete v tématech [kategorie koncového bodu microsoft 365 a webová služba IP adresa a URL microsoft 365](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
