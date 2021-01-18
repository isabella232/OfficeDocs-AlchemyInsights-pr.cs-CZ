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
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884912"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Přiřazení skupin k roli Azure AD

Pokud chcete skupině Azure AD s zdrojem oprávnění v Azure AD přiřadit roli Azure AD, postupujte takto:

1. Vytvořit novou skupinu vytvoří novou skupinu:

    a. Přihlaste se do centra pro správu Azure AD s oprávněním **správce rolí** nebo **globálního správce** .
    b. Vyberte **skupiny služby Azure Active Directory > > všechny skupiny > novou skupinu**.
    c. Vytvořte skupinu.

2. Přiřaďte roli skupině při vytváření skupiny nebo po vytvoření skupiny.

    a. Pokud chcete skupině přiřadit roli při vytváření skupiny, přepněte na přepínač **role služby Azure AD do skupiny** a vytvořte skupinu.
    b. Pokud chcete přiřadit roli skupině po jejím vytvoření, přejděte na kartu **přiřazené role** pro nově vytvořenou skupinu a přiřaďte roli skupině.  

**Správa členství ve skupině, která je přiřazená k roli Azure AD**

Abyste předešli zvýšení oprávnění, můžou ve výchozím nastavení měnit členství ve skupině, která je přiřazená k roli, jenom správcům rolí a globálních správcům. Mohou však zvolit přiřazení vlastníka takové skupiny a delegovat tento úkol.

Další informace o přiřazování cloudových skupin k rolím Azure AD najdete v tématu [přiřazení rolí služby AD ke skupině cloudu](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Další informace o rolích řešení potíží přiřazených ke skupinám cloudu najdete v tématu [řešení potíží s rolemi přiřazenými cloudovým skupinám](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





