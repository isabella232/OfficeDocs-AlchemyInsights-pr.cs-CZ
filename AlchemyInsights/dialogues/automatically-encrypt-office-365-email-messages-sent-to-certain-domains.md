---
title: Automatické šifrování e-mailových zpráv Office 365 posílaných na určité domény
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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524002"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Automatické šifrování e-mailových zpráv Office 365 posílaných na určité domény

1. V Centru [pro správu Exchange zvolte](https://outlook.office365.com/ecp/) **tok pošty a > pravidla.** 
2. Klikněte na **ikonu Nový (+)** a potom klikněte na Použít šifrování zpráv **Office 365 a ochranu přístupových práv u zpráv.**
3. Do **pole** Název zadejte název pravidla, například Šifrovat zprávy odesílané *contoso.com.*
4. V **části Použít toto pravidlo** v případě, že > domény **příjemce.** 
5. Zadejte název domény, například **contoso.com.**
6. Klikněte na ikonu Přidat **(+)** a potom na **OK.**
7. Vedle pole **Provést následující klikněte** na Vybrat jednu z **nich.** 
8. V rozevírací **nabídce šablony RMS** vyberte **Šifrovat** a potom klikněte na **OK.** (Pokud tuto možnost nevidíte, znamená to, že váš plán nezahrnuje automatické šifrování. Můžete ho ale přidat!)
9. Zvolte libovolný volitelný výběr (ze seznamu volitelných výběrů, které můžete v tomto okamžiku provést, z nichž mnohé mohou být ponechány s výchozím nastavením pro jednoduchost).
10. Klikněte na **Uložit**.

> [!IMPORTANT]
> Toto pravidlo můžete později zase vrátit a upravit.

Další informace o vytváření pravidel pro šifrování najdete v článku Definice pravidel toku pošty pro šifrování e-mailových zpráv v [Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)