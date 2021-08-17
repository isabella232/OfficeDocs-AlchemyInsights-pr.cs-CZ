---
title: Poradce při potížích se zprávami o odepření přístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085221"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Poradce při potížích se zprávami o odepření přístupu v Centru OneDrive pro správu SharePointu/Windows

Pokud se vám při pokusu o procházení Centra pro správu Sharepointu/OneDrive zobrazí zpráva o odepření přístupu, ujistěte se prosím, že jste uživateli [přiřadili licenci.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Pokud má uživatel licenci, měli byste se také ujistit, že má přiřazenou [roli](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) správce, která má přístup k centru pro správu.

K tomuto problému může dojít také při odstranění a opětovném vytvoření uživatele se stejným hlavním názvem uživatele (UPN). Nový účet se vytvoří pomocí jiné hodnoty PUID (Passport Unique ID). Když se uživatel pokusí získat přístup k kolekci webů nebo OneDrive, má uživatel nesprávný KÓD PUID. Druhý scénář zahrnuje synchronizaci adresářů s organizační jednotkou služby Active Directory (OU). Pokud se uživatelé už přihlásili k SharePoint a pak se přesunou do jiné OU a znovu se synchronizuje s SharePoint, může docházet k tomuto problému.

Pokud chcete tento problém vyřešit, měli byste obnovit původní hlavní název uživatele pomocí kroků v článku Obnovení [uživatele v Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Poznámka: Pokud OneDrive nebo SharePoint správce není k dispozici pro více uživatelů, kteří dřív měli přístup, může dojít k dočasnému problému se službou.  [Zkontrolujte řídicí panel stavu služby](https://portal.office.com/adminportal/home#/servicehealth).


