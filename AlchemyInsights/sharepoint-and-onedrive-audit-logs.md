---
title: Klasické sestavy protokolu auditování služby SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662201"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Protokoly auditování SharePointu a OneDrivu

## <a name="sharepoint-classic-audit-logs"></a>Protokoly auditování klasické verze SharePointu

SPO starší auditování bylo migrováno do protokolu Unified audit (UAL). Všechny SPO sestavy auditování starší verze teď budou napájeny přes UAL a starší signály auditu byly migrovány do UAL.

Klíčové změny:

* Střih není k dispozici jako možnost.
* Výběr konkrétních událostí k auditování není k dispozici. V [tomto dokumentu](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) najdete úplný seznam auditovaných událostí, které jsou ve výchozím nastavení dostupné.
* Možnost **umístění** v části **přizpůsobené sestavy** není dostupná.
* Možnost **otevřít nebo stáhnout dokumenty** není dostupná.

[Konfigurace nastavení auditování pro kolekci webů](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Moderní protokoly pro jednotné auditování v SharePointu a OneDrivu

* [Zapnutí nebo vypnutí protokolování jednotného auditu](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

V SharePointu nebo OneDrivu se nevyžaduje žádná další konfigurace.

Použití vyhledávání protokolování auditu ke kontrole aktivit souborů, složek, uživatelů, oprávnění:

* [Aktivity se soubory a stránkami](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Aktivity složky](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Aktivity sdílení a žádostí o přístup](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Aktivity synchronizace](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktivity správy webu](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Další informace o tom, jak tyto události získat, najdete v tématu [vyhledání protokolu auditování](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
