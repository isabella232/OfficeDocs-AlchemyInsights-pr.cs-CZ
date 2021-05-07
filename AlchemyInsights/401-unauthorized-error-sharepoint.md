---
title: 401 Neoprávněná chyba v SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233491"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Neoprávněná chyba v SharePoint

Pokud se v aplikaci SharePoint zobrazí chyba "(401) Neautorizované", může to souviset s vymazáváním tls 1.0/1.1. Další informace najdete v článcích:

[Připravuje se na TLS 1.2 v Office 365 a Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[Pokud klient nepodporuje tls 1.2, dochází k chybám ověřování.](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Pokud jsou uživatelé na Windows 7, zkontrolujte, jestli zaškrtá [tls cipher Suites v Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).