---
title: V aplikaci SharePoint došlo k chybě při zavření základního SharePoint
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
ms.openlocfilehash: 1b4f336f389eb6fd81ac2ca40e6047184cc4c1bf
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317689"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Chyba "Podkladové připojení bylo zavřené" v SharePoint

Pokud se v aplikaci SharePoint zobrazí chybová zpráva "Základní připojení bylo zavřené", může to souviset s vymazáváním protokolu TLS 1.0/1.1. Další informace najdete v těchto článcích:

- [Připravuje se na TLS 1.2 v Office 365 a Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Pokud klient nepodporuje tls 1.2, dochází k chybám ověřování.](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Aktualizace pro povolení tls 1.1 a TLS 1.2 jako výchozích zabezpečených protokolů ve WinHTTP v Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Pokud jsou uživatelé na Windows 7, zkontrolujte, jestli zaškrtá [tls cipher Suites v Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).