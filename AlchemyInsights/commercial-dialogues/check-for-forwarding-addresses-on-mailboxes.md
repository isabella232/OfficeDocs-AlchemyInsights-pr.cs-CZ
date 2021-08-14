---
title: Kontrola přeposílání adres v poštovních schránkách
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: a67305ed92e181f0ddfc5a929e8fe9631ceefdc99dea34118bc99975461f3868
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005803"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a>Kontrola přeposílání adres v poštovních schránkách

Někdy hackeři přeposílání e-mailových zpráv uživatelů sami sobě, takže nejdřív zkontrolujeme přeposílání adres a pravidel pro poštovní schránku. Pak zkontrolujeme protokoly auditování. Tady je postup, jak zkontrolovat přeposílání adres:

1. Vyberte **Uživatelé**  >  **aktivní uživatelé**.
1. Vyberte uživatele, jehož účet byl ohrožen.
1. V plovoucím seznamu, který se zobrazí, rozbalte **Mail Nastavení** a potom klikněte **na Upravit** pro **přeposílání e-mailů.**
1. Odeberte všechny adresy pro přeposílání, které nepoznáváte.