---
title: Zakázání tls1.0 a TLS 1.1 pro odeslání klienta SMTP AUTH
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/18/2021
ms.locfileid: "58454580"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>Zakázání tls1.0 a TLS 1.1 pro odeslání klienta SMTP AUTH

Nedávno jsme začali zakazovat tls1.0 a TLS 1.1 pro odesílání klientů SMTP AUTH. 

Pokud jste nakonfigurovali zařízení, aplikaci nebo server, který odesílá e-maily do Microsoft 365 pomocí metody odeslání klienta SMTP AUTH, zkontrolujte, jestli vaše zařízení, aplikace nebo server podporují protokol TLS 1.2 pro smtp. 