---
title: Poradce při potížích s kódy chyb ověřování a autorizace Azure AD (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035198"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Poradce při potížích s kódy chyb ověřování a autorizace Azure AD (AADSTS)

Pokud chcete vyřešit kódy chyb ověřování a autorizace služby AADSTS, proveďte následující doporučené kroky:

1. **Zpracování kódů chyb ve vaší aplikaci**

- **OAuth2.0 spec**, poskytuje pokyny, jak zpracovat chyby při ověřování pomocí chybové https://tools.ietf.org/html/rfc6749#section-5.2 části chybové odpovědi.

    - **Chyba:** Řetězec kódu chyby, který se používá ke klasifikaci typů chyb, ke kterým dojde, a měl by být použit k reakci na chyby.
    - Chybové **pole** má několik možných hodnot – prohlédněte si odkazy dokumentace protokolu a specifikace OAuth 2.0, kde najdete další informace o konkrétních chybách a o tom, jak na ně reagovat.

- Tady je ukázková chybová odpověď:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Informace o aktuálním kódu chyby vyhledávání**

- Kódy chyb a zprávy se mohou změnit. Nejnovější informace najdete na stránce s popisy chyb AADSTS, opravami a https://login.microsoftonline.com/error některými navrhovanými alternativními řešeními.
- Můžete taky hledat kódy chyb [AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) a odstraňovat je, jak je uvedeno v článku Kódy chyb [ověřování a autorizace Azure AD.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)

3. **Získat nápovědu**

- [Možnosti podpory](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) a nápovědy pro vývojáře – Pokud potřebujete odpověď na otázku nebo pomoc při řešení problému, který není zahrnutý v naší dokumentaci, může být čas kontaktovat odborníky o pomoc. Tento článek obsahuje několik návrhů, jak získat odpovědi na vaše otázky při vývoji aplikací, které se integrují s platformou identit Microsoftu.








