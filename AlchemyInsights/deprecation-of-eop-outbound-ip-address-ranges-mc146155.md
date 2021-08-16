---
title: 1065 Deprecation of EOP outbound IP address rangesMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031255"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecation of EOP outbound IP address ranges

Zjistili jsme potenciální problém s vaší organizací, který (pokud není opravený 26. října 2018), může přerušit tok pošty do místních nebo externích cílů. Jak jsme již dříve sdělili, zjednodušuje se správa rozsahů IP adres, slučování rozsahů IP adres Exchange Online Protection (EOP), které se používají k odesílání a přijímání e-mailů mimo Microsoft 365. Naše analýza označuje, že jeden nebo více externích zdrojů e-mailů nebo cílů, které jste nakonfigurovali v konektorech toku pošty, nepřijímá připojení z rozsahů IP adres uvedených [tady](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Před 26. říjnem vystupte, abyste zajistili, že tyto zdroje a cíle budou přijímat připojení ke všem publikovaných [IP adresám EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)a ze všech publikovaných IP adres.

Další informace o této změně najdete v tématu Příspěvky v Centru zpráv [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)nebo [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Poznámka:** Pokud jste v minulosti pro aktualizace koncových bodů používali publikování IP adres nebo adres URL pomocí html, XML a RSS, měli byste taky migrovat do nových webových služeb pro automatizaci těchto typů aktualizací. Další informace najdete v tématu [Microsoft 365 koncových bodů a Microsoft 365 IP adresa](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)a webová služba URL .
