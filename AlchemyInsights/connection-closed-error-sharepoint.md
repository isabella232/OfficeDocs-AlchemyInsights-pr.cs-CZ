---
title: Základní připojení bylo v aplikaci SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044405"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Chyba "Podkladové připojení bylo zavřené" v SharePoint

Pokud se v aplikaci SharePoint zobrazí chybová zpráva "Základní připojení bylo zavřené", může to souviset s vymazáváním tls 1.0/1.1. Další informace najdete v těchto článcích:

- [Připravuje se na TLS 1.2 v Office 365 a Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Pokud klient nepodporuje tls 1.2, dochází k chybám ověřování.](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Aktualizace pro povolení tls 1.1 a TLS 1.2 jako výchozích zabezpečených protokolů ve WinHTTP v Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Pokud jsou uživatelé na Windows 7, zkontrolujte, jestli zaškrtá [tls cipher Suites v Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).