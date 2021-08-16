---
title: Přiřazení skupin k roli Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036233"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Přiřazení skupin k roli Azure AD

Pokud chcete přiřadit skupinu Azure AD se zdrojem autority v Azure AD k roli Azure AD, postupujte takto:

1. Vytvoření nové skupiny – Vytvoření nové skupiny:

    a. Přihlaste se do Centra pro správu Azure AD s **oprávněními** správce rolí nebo **globálního správce.**
    b. Vyberte **Azure Active Directory > Skupiny > Všechny skupiny > Nová skupina**.
    c. Vytvořte skupinu.

2. Přiřaďte roli skupině buď během vytváření skupiny, nebo po vytvoření skupiny.

    a. Pokud chcete přiřadit roli skupině v okamžiku vytvoření skupiny, zapněte přepínač **Role Azure AD,** který se skupině může přiřadit, a vytvořit skupinu.
    b. Pokud chcete přiřadit roli skupině po vytvoření,  přejděte pro nově vytvořenou skupinu na kartu Přiřazené role a přiřaďte ji skupině.  

**Správa členství ve skupině, která je přiřazená k roli Azure AD**

Aby se zabránilo zvýšení oprávnění, můžou ve výchozím nastavení změnit členství skupiny přiřazené k roli jenom správci rolí s oprávněními a globální správci. Mohou se ale rozhodnout, že pro takovou skupinu přiřadí vlastníka a deleguje tento úkol.

Další podrobnosti o přiřazování cloudových skupin k rolím Azure AD najdete v tématu Přiřazení [rolí AD cloudové skupině](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Další podrobnosti o odstraňování rolí přiřazených cloudovým skupinám najdete v tématu Řešení potíží s [rolemi přiřazenými cloudovým skupinám.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





