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
ms.openlocfilehash: 8935f461aaf24cb100516311203ef642f5dbed931e472df944c1cd7e72a8cf4e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890259"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Neoprávněná chyba v SharePoint

Pokud se v aplikaci SharePoint zobrazí chyba "(401) Neautorizované", může to souviset s vymazáváním TLS 1.0/1.1. Další informace najdete v článcích:

- [Připravuje se na TLS 1.2 v Office 365 a Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Pokud klient nepodporuje tls 1.2, dochází k chybám ověřování.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Aktualizace pro povolení tls 1.1 a TLS 1.2 jako výchozích zabezpečených protokolů ve WinHTTP v Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Pokud jsou uživatelé na Windows 7, zkontrolujte, jestli v 7 Windows [TLS Cipher Suites.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)