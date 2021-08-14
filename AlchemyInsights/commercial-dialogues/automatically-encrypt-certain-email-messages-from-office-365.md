---
title: Automatické šifrování určitých e-mailových zpráv z Office 365
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
ms.openlocfilehash: 74f9733196004fd7a78eeb290c948a9f35ac2a31b3c5b00bf82e44081aac8637
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988828"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Automatické šifrování určitých e-mailových zpráv z Office 365

1. V Centru [Exchange správy](https://outlook.office365.com/ecp/)zvolte **tok pošty a > pravidla**. 
2. Klikněte na **ikonu Nový (+)** a potom klikněte na Použít Šifrování zpráv Office 365 a ochranu **práv u zpráv**.
3. Do **pole** Název zadejte název pravidla, například *Zašifrovat všechny zprávy*.
4. V **části Použít toto pravidlo, pokud** zvolte **[Použít u všech zpráv]**. 
5. Vedle pole **Do the following (Provést následující)** klikněte na Select one **(Vybrat jednu).** 
6. V rozevírací **nabídce šablony RMS** vyberte Šifrovat a potom klikněte na **OK.**  (Pokud tuto možnost nevidíte, znamená to, že váš plán neobsahuje automatické šifrování. Ale můžete ho přidat!)
7. Zaškrtněte políčko **Auditovat toto pravidlo s úrovní závažnosti** a pak vyberte požadovanou úroveň. Pokud má vaše společnost smluvní závazky posílat všechny e-maily zašifrované, doporučujeme nastavit úroveň **Vysoká.**
8. V **části Zvolit model pro toto pravidlo** klikněte na **Vynutit**. 
9. Zvolte libovolný volitelný výběr (ze seznamu volitelných výběrů, které můžete v tomto okamžiku provést, z nichž mnohé můžete nechat s výchozím nastavením pro jednoduchost).
10. Klikněte na **Uložit**.

> [!IMPORTANT]
> Toto pravidlo se můžete vrátit a toto pravidlo upravit později.

Další informace o vytváření pravidel pro šifrování najdete v tématu Definování pravidel toku pošty pro šifrování e-mailových zpráv [v Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

