---
title: Protokoly hesel
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50524118"
---
# <a name="password-logs"></a>Protokoly hesel

**Mám problémy s přístupem k protokolům auditování při resetování hesla**

Pokud chcete vyřešit problémy s přístupem k protokolům auditování resetování hesla, proveďte následující krok:

Ujistěte se, že máte oprávnění k zobrazení protokolů auditování. 

Autorizované jsou jenom tyto role:
 - Globální správce
 - Správce zabezpečení
 - Čtenář zabezpečení

**Chci zobrazit všechny události auditování resetování hesel od okamžiku, kdy jsem ho poprvé nasazoval(a).**

V sestavách za posledních 30 dní se uloží až 120 000 událostí pro resetování/registraci hesel. Tento maximální limit platí pro uživatelské rozhraní při stahování souboru CSV. Přes PowerShell je dostupný 1 milion událostí.
Další informace najdete pod následujícími odkazy:

- [Události samoobslužného resetování hesla z rozhraní API sestav a událostí Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Jak rychle stáhnout události registrace resetování hesla pomocí PowerShellu](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Chci se dozvědět víc o možnostech vytváření sestav pro resetování hesel**

Zkontrolujte, kdo registruje nebo resetuje hesla pomocí protokolů auditování hesel Azure AD na portálu Azure Portal v části Uživatelé a **skupiny.**
Další informace najdete na těchto odkazech:

- [Přehled sestav resetování hesla](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Jak zobrazit sestavy pro resetování hesla na portálu Azure Portal](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Události samoobslužného resetování hesla z rozhraní API sestav a událostí Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Jak rychle stáhnout události registrace resetování hesla pomocí PowerShellu](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


