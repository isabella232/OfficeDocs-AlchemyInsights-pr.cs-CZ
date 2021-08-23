---
title: Moje aplikace se nezobrazuje v správného řízení aplikací
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454467"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Moje aplikace se nezobrazuje v správného řízení aplikací

Pokud se vaše aplikace nezobrazuje v správného řízení aplikací, podívejte se na toto:

1. Přejděte na [Azure AD a](https://aad.portal.azure.com/) vyhledejte ID aplikace pro vaši aplikaci vyhledáním názvu aplikace na horním panelu na stránce Přehled.

1. Access Graph Exploreru a vyhledejte ID aplikace v rámci vašeho hlavního objektu služby pomocí tohoto dotazu a nahraďte ho příslušným <appId> ID aplikace: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Pokud nejsou vráceny žádné výsledky, vyhledejte ID aplikace v aplikaci pomocí tohoto dotazu a nahraďte ho příslušným <appId> ID aplikace: < https://graph.microsoft.com/v1.0/applications? $search= "id aplikace: <appId> ">

Pokud máte s dotazem problémy, podívejte se na informace [v tématu Získání podpory](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Další informace nebo přehled o vašich aplikacích v nástroji Řízení aplikací najdete v tématu Informace o viditelnosti a [přehledech.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Další informace o prohlížení aplikací najdete v tématu [Zobrazení aplikací](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps).
