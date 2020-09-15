---
title: Řešení potíží s synchronizací hesel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664919"
---
# <a name="troubleshoot-password-synchronization"></a>Řešení potíží s synchronizací hesel

Chcete-li vyřešit problémy se synchronizací hesel, začněte pomocí tohoto úkolu AAD Connect pro řešení potíží zjistit, proč se hesla nesynchronizují. Začněte tím, že přejdete na [Správa přímé synchronizace](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Na serveru Azure AD Connect otevřete novou relaci Windows PowerShellu a vyberte možnost **Spustit jako správce** .

2. Spusťte Set-ExecutionPolicy RemoteSigned nebo Set-ExecutionPolicy Unrestricted.

3. Spusťte Průvodce Azure AD Connect.

4. Přejděte na stránku další úkoly > **řešení potíží**  >  **Next**.

5. Výběrem možnosti **Spustit** otevřete nabídku odstraňování potíží PowerShellu.

6. Vyberte **Poradce při potížích s synchronizací hesel**.

    Problém se obvykle nesynchronizuje s heslem pro konkrétní uživatelský účet.

    **Poznámky** Synchronizace hesel se nezdaří, pokud uplynula Poslední úspěšná synchronizace hesla.

Další nápovědu k řešení potíží s synchronizací hesel najdete v článku [Poradce při synchronizaci hash synchronizace s heslem pomocí synchronizace Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).