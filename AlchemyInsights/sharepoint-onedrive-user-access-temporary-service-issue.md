---
title: Problémy s výkonem SharePoint nebo OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093683"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint nebo OneDrive pomalé, nepřístupné nebo nedostupné pro více uživatelů

Pokud OneDrive nebo SharePoint není dostupný pro více uživatelů, kteří k tomu měli přístup dřív, může dojít k dočasnému problému se službou. [Zkontrolujte řídicí panel stavu služby](https://portal.office.com/adminportal/home#/servicehealth).

**Přidání a licence uživatele**

Ujistěte se, [že přiřaďte](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)licence uživatelům v Microsoft 365 pro firmy .


**Přiřazení oprávnění**

Pokud má uživatel přiřazenou licenci na SharePoint a stále dostává zprávu o odepření přístupu, ujistěte se prosím, že má přiřazenou [odpovídající úroveň](https://docs.microsoft.com/sharepoint/understanding-permission-levels) oprávnění.

**Zvažte použití funkce žádosti o přístup.**

Funkce [žádosti o přístup](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umožňuje uživatelům požádat o přístup k obsahu, který momentálně nemají oprávnění k zobrazení.

**Povolit vlastní skript může způsobit problémy s odepřením přístupu**

Existují určité scénáře, kdy funkce Povolit vlastní *skript* může prezentovat odepřený přístup. Seznam ovlivněných funkcí, důležité informace o zabezpečení a možnost tuto funkci zakázat Navštivte prosím [povolit nebo zabránit vlastnímu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

