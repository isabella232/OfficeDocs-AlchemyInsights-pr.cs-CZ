---
title: Automatické šifrování e-mailových zpráv Office 365 odeslaných do určitých domén
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744549"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Automatické šifrování e-mailových zpráv Office 365 odeslaných do určitých domén

1. V Centru [pro správu Exchange](https://outlook.office365.com/ecp/)zvolte **tok pošty > pravidla**. 
2. Klikněte na **ikonu Nový (+)** a potom klikněte na Použít šifrování zpráv **Office 365** a ochranu práv u zpráv.
3. Do **pole** Název zadejte název pravidla, například Šifrovat zprávy odeslané *contoso.com.*
4. V **části Použít toto pravidlo, pokud** zvolte > doména **je**. 
5. Zadejte název domény, například **contoso.com**.
6. Klikněte na **ikonu Přidat (+)** a potom klikněte na **OK.**
7. Vedle pole **Do the following (Provést následující)** klikněte na Select one **(Vybrat jednu).** 
8. V rozevírací **nabídce šablony RMS** vyberte Šifrovat a potom klikněte na **OK.**  (Pokud tuto možnost nevidíte, znamená to, že váš plán neobsahuje automatické šifrování. Ale můžete ho přidat!)
9. Zvolte libovolný volitelný výběr (ze seznamu volitelných výběrů, které můžete v tomto okamžiku provést, z nichž mnohé můžete nechat s výchozím nastavením pro jednoduchost).
10. Klikněte na **Uložit**.

> [!IMPORTANT]
> Toto pravidlo se můžete vrátit a toto pravidlo upravit později.

Další informace o vytváření pravidel pro šifrování najdete v článku Definování pravidel toku pošty pro šifrování e-mailových zpráv [v Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)