---
title: Určení IP adresy a klienta v protokolech auditování
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 57a1756787f8297a2a1ab3012b95aaa2f33e6045
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313012"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Určení IP adresy a klienta v protokolech auditování

IP adresa, která odpovídá aktivitě uživatele Microsoft 365 nebo správce, se zobrazí v protokolech auditování. Zaprotokoluje se taky informace o klientovi. Tady jsou kroky k identifikaci těchto informací.

1. Přihlaste se do [centra Microsoft 365 dodržování předpisů](https://protection.office.com/).

2. Přejděte na **vyhledávací stránku protokolu**  >  **auditování** hledání.

   Pokud vás zajímá určitá aktivita, vyberte ji ze **seznamu** Aktivity. Pokud ne, vrátí se všechny aktivity vybranému uživateli (výchozí nastavení).

   **Poznámka:** Některé aktivity nemusí být dostupné v nabídce **Aktivity.** Tyto položky auditování se ale vrátí, pokud je **vybrána** možnost Zobrazit výsledky pro všechny aktivity (výchozí nastavení).

3. Zadejte uživatelské jméno do **pole Uživatelé,** vyberte odpovídající rozsah dat pro aktivitu a potom klikněte na **Hledat.**

Ve výsledcích uvidíte IP adresu této aktivity v podokně výsledků. Výběrem záznamu auditování zobrazíte  podrobné informace v informačním seznamu Podrobnosti (například Klient, Uživatel, který provedl akci atd.).

Další informace najdete v tématu Vyhledání IP adresy počítače, který se používá pro přístup k [ohroženému účtu](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
