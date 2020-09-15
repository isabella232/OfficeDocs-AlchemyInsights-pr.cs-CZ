---
title: Jak zakázat externí skupiny
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704121"
---
# <a name="how-to-disable-external-groups"></a>Jak zakázat externí skupiny

Externí zasílání zpráv Yammeru používá pravidla přenosu Exchange (vynucovat), což je sada proaktivních ovládacích prvků, které brání sdílení informací o společnosti. Aby uživatelé mohli vytvářet externí skupiny, musíte nakonfigurovat pravidlo přenosu Exchange (ETR) a potom Yammer nakonfigurovat tak, aby používal pravidlo přenosu Exchange pro blokování externích zpráv.
  
Po vytvoření pravidla v centru pro správu Exchange Online nastavte ETR na použít v Yammeru takto:
  
- Přihlaste se k Yammeru jako ověřený správce a v **centru pro správu Yammeru**přejděte na obsah C **a \> nastavení zabezpečení.**

- V části **externí zasílání zpráv**vyberte **v Yammeru vynutit pravidla přenosu Exchange Online (vynucovat).**

- Zvolte **Uložit**.

Další informace najdete v článku [zakázání externího zasílání zpráv v síti Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  