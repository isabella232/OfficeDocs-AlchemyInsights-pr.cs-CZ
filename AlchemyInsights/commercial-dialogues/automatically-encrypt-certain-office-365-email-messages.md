---
title: Automatické šifrování určitých Office 365 e-mailových zpráv
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
ms.openlocfilehash: b15a72ced4921b3df1b7105837592781188a2a25
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327967"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Automatické šifrování určitých Office 365 e-mailových zpráv

Zprávy, které uživatelé odesílat určitým externím lidem nebo organizacím, můžete automaticky šifrovat. Postupujte takto:

1. V Centru [Exchange správy](https://outlook.office365.com/ecp/)zvolte **tok pošty a > pravidla**. 
2. Klikněte na **ikonu Nový (+)** a potom klikněte na Použít Šifrování zpráv Office 365 a ochranu **práv u zpráv**.
3. Do **pole** Název zadejte název pravidla, například Šifrovat zprávy odeslané *DrToniRamos@gmail.com.*
4. V **části Použít toto pravidlo, pokud** zvolte > je tato **osoba**. 
5. V okně **Vybrat členy** vyberte jméno osoby, pro kterou chcete použít pravidlo šifrování, a klikněte na **Přidat.** 
6. Až budete přidávání uživatelů hotovi, klikněte na **OK.**
7. Vedle pole **Do the following (Provést následující)** klikněte na Select one **(Vybrat jednu).** 
8. V rozevírací **nabídce šablony RMS** vyberte Šifrovat a potom klikněte na **OK.**  (Pokud tuto možnost nevidíte, znamená to, že váš plán neobsahuje automatické šifrování. Ale můžete ho přidat!)
9. Zvolte libovolný volitelný výběr (ze seznamu volitelných výběrů, které můžete v tomto okamžiku provést, z nichž mnohé můžete nechat s výchozím nastavením pro jednoduchost).
10. Klikněte na **Uložit**.

**Důležité:** Toto pravidlo se vždycky můžete vrátit a upravit později.

Další informace o vytváření pravidel pro šifrování najdete v tématu Definování pravidel toku pošty pro šifrování e-mailových zpráv [v Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

