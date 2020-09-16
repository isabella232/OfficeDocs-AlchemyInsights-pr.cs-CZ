---
title: Poradce při potížích s odepřením přístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767651"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Řešení potíží s odepřením přístupu v centru pro správu SharePointu/OneDrivu

Pokud se při pokusu o přechod do centra pro správu SharePointu a OneDrivu zobrazuje zpráva o odepření přístupu, ujistěte se, že [uživateli přiřadíte licenci](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Pokud má uživatel licenci, měli byste také ověřit, že je jim [přiřazena role správce](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , která má přístup k centrům pro správu.

Tento problém může také nastat, když se uživatel odstraní a znovu vytvoří se stejným hlavním názvem uživatele (UPN). Nový účet je vytvořen pomocí jiného identifikátoru PUID (kód účtu služby Passport). Když se uživatel pokusí získat přístup ke kolekci webů nebo k OneDrivu, má nesprávný PUID. Druhý scénář zahrnuje synchronizaci adresářů s organizační jednotkou služby Active Directory. Pokud se uživatelé už přihlásili k SharePointu a pak jsou přesunuti na jinou organizační jednotku a znovu se synchronizují se SharePointem, může dojít k těmto potížím.

Tento problém vyřešíte tak, že obnovíte původní uživatelské jméno (UPN) pomocí kroků v tomto článku a [obnovíte uživatele v Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Poznámka: Pokud centrum pro správu OneDrivu nebo SharePointu není dostupné pro víc uživatelů, kteří mají přístup dřív, může se jednat o dočasný problém služby.  [Zkontrolujte řídicí panel stavu služeb](https://portal.office.com/adminportal/home#/servicehealth).


