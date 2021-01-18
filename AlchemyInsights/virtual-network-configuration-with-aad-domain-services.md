---
title: Virtuální konfigurace s doménovým službám AAD
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
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884976"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuální konfigurace s doménovým službám AAD

Virtuální konfigurace s doménou AAD zahrnuje následující kroky: 

1. Kontrola stavu vaší domény na Azure Portalu https://aka.ms/aadds-health
2. Kontrola NSG pravidel, která blokují porty potřebné k synchronizaci v Azure AD Domain Services na portálu https://aka.ms/aadds-networking
3. Ujistěte se, že je vaše virtuální síť nasazená ve stejné oblasti Azure jako doména spravovaná službou Azure AD Domain Services.
4. Ujistěte se, že nemáte ve virtuální síti k dispozici stejnou doménu s názvem domény.

Další podrobnosti o zvažování návrhu pro podporu služby DNS Virtual Network najdete v tématu [zvážení virtuální sítě](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

