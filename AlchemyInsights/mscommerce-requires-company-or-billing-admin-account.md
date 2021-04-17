---
title: Připojení k modulu MSCommerce
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829729"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce vyžaduje účet společnosti nebo správce fakturace.

Modul MSCommerce vyžaduje účet s oprávněními společnosti nebo správce fakturace. Pokud se zobrazí následující chyba, budete se muset znovu připojit k jinému účtu.

*ErrorMessage – Vzdálený server vrátil chybu: (403) Zakázáno. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Nepodařilo se zopakovat ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Chyba při zápisu], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Pokud váš účet nemá oprávnění společnosti nebo správce fakturace, obraťte se na správce IT.
