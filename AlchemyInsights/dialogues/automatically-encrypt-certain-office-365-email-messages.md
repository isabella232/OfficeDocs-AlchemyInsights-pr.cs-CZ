---
title: Automatické šifrování některých e-mailových zpráv Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524010"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Automatické šifrování některých e-mailových zpráv Office 365

Zprávy, které uživatelé pošlou určitým externím lidem nebo organizacím, můžete automaticky šifrovat. Postupujte takto:

1. V Centru [pro správu Exchange zvolte](https://outlook.office365.com/ecp/) **tok pošty a > pravidla.** 
2. Klikněte na **ikonu Nový (+)** a potom klikněte na Použít šifrování zpráv **Office 365 a ochranu přístupových práv u zpráv.**
3. Do **pole** Název zadejte název pravidla, například Šifrování zpráv odeslaných *DrToniRamos@gmail.com.*
4. V **části Použít toto pravidlo vyberte** Příjemce, > je tato **osoba.** 
5. V okně **Vybrat členy** vyberte jméno osoby, na kterou chcete pravidlo šifrování použít, a klikněte na **Přidat.** 
6. Po přidání uživatelů klikněte na **OK.**
7. Vedle pole **Provést následující klikněte** na Vybrat jednu z **nich.** 
8. V rozevírací **nabídce šablony RMS** vyberte **Šifrovat** a potom klikněte na **OK.** (Pokud tuto možnost nevidíte, znamená to, že váš plán nezahrnuje automatické šifrování. Můžete ho ale přidat!)
9. Zvolte libovolný volitelný výběr (ze seznamu volitelných výběrů, které můžete v tomto okamžiku provést, z nichž mnohé mohou být ponechány s výchozím nastavením pro jednoduchost).
10. Klikněte na **Uložit**.

> [!IMPORTANT]
> Toto pravidlo můžete později zase vrátit a upravit.

Další informace o vytváření pravidel pro šifrování najdete v článku Definice pravidel toku pošty pro šifrování e-mailových zpráv v [Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

