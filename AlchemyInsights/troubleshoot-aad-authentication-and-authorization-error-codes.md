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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="c57ad-102">Poradce při potížích s kódy chyb ověřování a autorizace Azure AD (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="c57ad-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="c57ad-103">Pokud chcete vyřešit kódy chyb ověřování a autorizace služby AADSTS, proveďte následující doporučené kroky:</span><span class="sxs-lookup"><span data-stu-id="c57ad-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="c57ad-104">**Zpracování kódů chyb ve vaší aplikaci**</span><span class="sxs-lookup"><span data-stu-id="c57ad-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="c57ad-105">**OAuth2.0 spec**, poskytuje pokyny, jak zpracovat chyby při ověřování pomocí chybové https://tools.ietf.org/html/rfc6749#section-5.2 části chybové odpovědi.</span><span class="sxs-lookup"><span data-stu-id="c57ad-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="c57ad-106">**Chyba:** Řetězec kódu chyby, který se používá ke klasifikaci typů chyb, ke kterým dojde, a měl by být použit k reakci na chyby.</span><span class="sxs-lookup"><span data-stu-id="c57ad-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="c57ad-107">Chybové **pole** má několik možných hodnot – prohlédněte si odkazy dokumentace protokolu a specifikace OAuth 2.0, kde najdete další informace o konkrétních chybách a o tom, jak na ně reagovat.</span><span class="sxs-lookup"><span data-stu-id="c57ad-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="c57ad-108">Tady je ukázková chybová odpověď:</span><span class="sxs-lookup"><span data-stu-id="c57ad-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="c57ad-109">**Informace o aktuálním kódu chyby vyhledávání**</span><span class="sxs-lookup"><span data-stu-id="c57ad-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="c57ad-110">Kódy chyb a zprávy se mohou změnit.</span><span class="sxs-lookup"><span data-stu-id="c57ad-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="c57ad-111">Nejnovější informace najdete na stránce s popisy chyb AADSTS, opravami a https://login.microsoftonline.com/error některými navrhovanými alternativními řešeními.</span><span class="sxs-lookup"><span data-stu-id="c57ad-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="c57ad-112">Můžete taky hledat kódy chyb [AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) a odstraňovat je, jak je uvedeno v článku Kódy chyb [ověřování a autorizace Azure AD.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)</span><span class="sxs-lookup"><span data-stu-id="c57ad-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="c57ad-113">**Získat nápovědu**</span><span class="sxs-lookup"><span data-stu-id="c57ad-113">**Get Help**</span></span>

- <span data-ttu-id="c57ad-114">[Možnosti podpory](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) a nápovědy pro vývojáře – Pokud potřebujete odpověď na otázku nebo pomoc při řešení problému, který není zahrnutý v naší dokumentaci, může být čas kontaktovat odborníky o pomoc.</span><span class="sxs-lookup"><span data-stu-id="c57ad-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="c57ad-115">Tento článek obsahuje několik návrhů, jak získat odpovědi na vaše otázky při vývoji aplikací, které se integrují s platformou identit Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="c57ad-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








