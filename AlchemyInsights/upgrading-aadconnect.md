---
title: 932 upgrade AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806032"
---
# <a name="upgrade-azure-ad-connect"></a>Upgrade služby Azure AD Connect

Ve výchozím nastavení je automatický upgrade povolený pro Azure AD Connect, který vám pomůže zajistit, že máte nejnovější verzi. Pokud chcete ověřit nastavení automatického upgradu, použijte rutinu **Get-ADSyncAutoUpgrade** v Azure AD. Rutina vrátí jednu z následujících hodnot:

- **Povoleno**: je povolen automatický upgrade.

- **Zakázáno**: automatický upgrade je zakázán.

- **Pozastaveno**: systém už neumožňuje přijímat automatické upgrady. Tuto hodnotu nemůžete nakonfigurovat. je nastavená systémem.

Další informace najdete v tématu [Automatický upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Pokud chcete stáhnout nejnovější verzi Azure AD Connect, přejděte na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
