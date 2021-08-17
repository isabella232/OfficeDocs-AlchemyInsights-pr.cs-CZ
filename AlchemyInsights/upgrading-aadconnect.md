---
title: 932 Upgrade AADConnect
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
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104805"
---
# <a name="upgrade-azure-ad-connect"></a>Upgrade služby Azure AD Připojení

Ve výchozím nastavení je pro Azure AD Připojení povolen automatický upgrade, což pomáhá zajistit, že používáte nejnovější verzi. K ověření nastavení automatického upgradu použijte **rutinu Get-ADSyncAutoUpgrade v** Azure AD PowerShellu. Rutina vrátí jednu z následujících hodnot:

- **Povoleno:** Je povolen automatický upgrade.

- **Zakázáno:** Automatický upgrade je zakázaný.

- **Pozastaveno:** Systém už nemá nárok na automatické upgrady. Tuto hodnotu nemůžete nakonfigurovat. je nastavený systémem.

Další informace najdete v tématu [Automatický upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Pokud si chcete stáhnout nejnovější verzi služby Azure AD Připojení, přejděte na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
