---
title: Poradce při potížích se zprávami s odepření přístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707947"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Poradce při potížích se zprávami o odepření přístupu v Centru pro správu SharePointu nebo OneDrivu

Pokud se vám při pokusu o procházení do Centra pro správu SharePointu nebo OneDrivu zobrazí zpráva o odepření přístupu, ujistěte se, že jste uživateli [přiřadili licenci.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Pokud má uživatel licenci, měli byste se ujistit, že má přiřazenou [roli](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) správce, která má přístup k centrem pro správu.

K tomuto problému může také dojít, když se uživatel odstraní a znovu vytvoří se stejným hlavním názvem uživatele (UPN). Nový účet se vytvoří pomocí jiné hodnoty ID uživatelského účtu (Passport Unique ID). Když se uživatel pokusí o přístup ke kolekci webů nebo k jejich OneDrivu, má uživatel nesprávný KÓD PUID. Druhý scénář zahrnuje synchronizaci adresářů s organizační jednotkou služby Active Directory. Pokud se už uživatelé přihlásili k SharePointu a pak se přesunou do jiné OU a budou se znovu synchronizovat se SharePointem, mohou zaznamenat tento problém.

Tento problém vyřešíte tak, že obnovíte původní hlavní název uživatele pomocí postupu v článku Obnovení [uživatele v Microsoftu 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Poznámka: Pokud není Centrum pro správu OneDrivu nebo SharePointu dostupné více uživatelům, kteří k přístupu měli předtím přístup, může jít o dočasný problém se službou.  [Zkontrolujte řídicí panel stavu služby.](https://portal.office.com/adminportal/home#/servicehealth)


