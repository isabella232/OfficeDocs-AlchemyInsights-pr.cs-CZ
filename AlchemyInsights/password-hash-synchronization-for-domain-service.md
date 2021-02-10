---
title: Synchronizace hodnot hash hesel u služby domény
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177383"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Synchronizace hodnot hash hesel u služby domény

**Pokud instance Azure služba AD DS vás vyzve k povolení synchronizace hodnot hash hesel**

Narazíte na scénář, ve kterém používáte hybridní prostředí s uživateli, kteří se synchronizují z místního prostředí Azure služba Active Directory Domain Services (služba AD DS). Tento scénář se setkávají i přes to, že máte synchronizaci hodnot hash hesel z místní služba AD DS do vašeho tenanta Azure AD.

Tato část obsahuje přehledné informace o problému a osobě, která ho má odstranit. Na obrázku vidíte tři základní strany v transakci e-mailu Office 365 - odesílatele, Office 365 a příjemce. Červeně označená oblast je oblast, ve které je obvykle potřeba problém odstranit.

K tomu dochází proto, že Azure AD Connect ve výchozím nastavení nesynchronuje starší hodnoty hash hesel NTLM (New Technology LAN Manager) a Kerberos, které jsou potřeba pro Azure služba AD DS.

**Řešení** 

Aby bylo možné synchronizovat tyto a hash hesel požadované pro ověřování NTLM a Kerberos, bude potřeba nakonfigurovat Azure AD Connect.

Po nakonfigurování Azure AD Connect pak místní událost pro vytvoření účtu nebo změnu hesla také synchronizuje starší hash hesel do Azure AD. V tomto [článku najdete](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) další informace a pokyny k povolení synchronizace hesel v hybridním prostředí Azure služba AD DS Azure.