---
title: 646 Jak nakonfigurovat AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963636"
---
# <a name="configure-sync-features"></a>Konfigurace funkcí synchronizace

Azure AD Připojení obsahuje několik funkcí, které jsou ve výchozím nastavení povolené nebo které můžete povolit později. Některé funkce vyžadují další konfiguraci v určitých prostředích.

- [Filtrování omezuje,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) že se objekty synchronizují s Azure AD. Ve výchozím nastavení se synchronizují všichni uživatelé, kontakty, skupiny Windows 10 účty počítačů. Můžete zahrnout nebo vyloučit objekty založené na doménách, OU nebo jiných atributech.

- [Synchronizace hodnot hash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) hesel synchronizuje hodnotu hash hesel z místního adresáře Active Directory do Azure AD. To umožňuje správu hesel na jednom místě, ale použití stejného hesla v místním i cloudovém prostředí. Vzhledem k tomu, že služba Active Directory je autoritativním zdrojem, můžete použít vlastní zásady hesel.

- [Samoobslužné resetování hesla (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umožňuje uživatelům resetovat vlastní hesla v cloudu a přitom používat místní zásady hesel.

- [Zpětný zápis zařízení](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umožňuje zaregistrovaná zařízení v Azure AD zapisovat zpátky do místního adresáře Active Directory, aby je bylo možné použít pro podmíněný přístup.

- [Zabránění náhodným odstraněním](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je ve výchozím nastavení povolené, aby se zabránilo příliš mnoha současným odstraněním objektů (více než 500 objektů na synchronizaci). Toto nastavení můžete změnit tak, aby splňovalo potřeby vaší organizace.

- [Automatický upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je ve výchozím nastavení povolený pro expresní instalace a pomáhá zajistit, aby vaše verze služby Azure AD Připojení vždy aktuální.
