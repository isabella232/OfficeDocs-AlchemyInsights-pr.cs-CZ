---
title: Stav domény – nejsou vybrány žádné služby.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 2247da07d60431edef5b5dea8a5c06d51579008c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326570"
---
# <a name="domain-status---no-services-selected"></a>Stav domény – nejsou vybrány žádné služby.

**Žádné vybrané** služby znamená, že jste nevy vybrali žádné služby Microsoft 365, jako je Exchange Online, Skype pro firmy nebo Intune a Správa mobilních zařízení pro Microsoft 365 pro použití s vaší vlastní doménou. Pokud používáte místní hybridní Exchange (Exchange s Exchange Online) nebo externí filtrování spamu s Exchange a žádným jiným služby Microsoft, můžete tuto zprávu ignorovat. Stav domény je dostupný jenom u domén připojených přímo ke službě.

Výběr služeb pro vaši doménu:

1. V **Nastavení**  >  [**Domény**](https://admin.microsoft.com/Adminportal/Home)zaškrtněte políčko vedle domény se stavovou zprávou Žádné **služby** vybrané .
1. Výběrem **možnosti Spravovat DNS** spusťte Průvodce nastavením domény.
    - Pokud **zvolíte Přidat vlastní záznamy DNS,** nezapomeňte po zobrazení výzvy vybrat službu. Další služby by mohly být dostupné v části **Upřesnit možnosti**.
    - Pokud zvolíte **Nechat Microsoft přidávat záznamy DNS** nebo Další **možnosti** Nastavení online služeb pro mě, všechny dostupné služby se navrhují a  >   vyberou automaticky.
1. Pokračujte v průvodci a dokončete nastavení DNS a možnosti služeb.
 
Další nápovědu k nastavení domény najdete v tématu [Přidání záznamů DNS pro připojení domény](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

