---
title: 646 jak nakonfigurovat AADConnect
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
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704482"
---
# <a name="configure-sync-features"></a>Konfigurace funkcí synchronizace

Azure AD Connect obsahuje několik funkcí, které jsou ve výchozím nastavení povolené, nebo je můžete povolit později. Některé funkce vyžadují další konfiguraci v konkrétních prostředích.

- [Filtrování](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) omezení: objekty jsou synchronizovány do služby Azure AD. Ve výchozím nastavení se synchronizují všichni uživatelé, kontakty, skupiny a účty počítačů s Windows 10. Můžete zahrnout nebo vyloučit objekty na základě domén, organizačních jednotek nebo jiných atributů.

- [Synchronizace hash hesla](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) : synchronizuje hodnotu hash hesla z místní služby Active Directory do Azure AD. To umožňuje správu hesel v jednom umístění, ale používat stejné heslo v místním i cloudovém prostředí. Protože je služba Active Directory autoritativním zdrojem, můžete použít vlastní zásady hesel.

- [Samoobslužné resetování hesla (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umožňuje uživatelům resetovat si svoje vlastní hesla v cloudu i při používání místních zásad hesel.

- [Zpětný zápis zařízení](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umožňuje, aby registrovaná zařízení v Azure AD byla zapsána zpátky do místní služby Active Directory, aby se mohla používat pro podmíněný přístup.

- Možnost [zabránit nechtěným odstraněním](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je ve výchozím nastavení zapnutá, aby se zabránilo přílišnému počtu současných odstranění objektů (více než 500 objektů na synchronizaci). Toto nastavení můžete změnit podle potřeb vaší organizace.

- [Automatický upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je ve výchozím nastavení povolený pro Expresní instalace a pomáhá zajistit, že vaše verze Azure AD Connect je vždycky aktuální.
