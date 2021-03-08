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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524014"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Automatické šifrování určitých e-mailových zpráv z Office 365

1. V Centru [pro správu Exchange zvolte](https://outlook.office365.com/ecp/) **tok pošty a > pravidla.** 
2. Klikněte na **ikonu Nový (+)** a potom klikněte na Použít šifrování zpráv **Office 365 a ochranu přístupových práv u zpráv.**
3. Do **pole** Název zadejte název pravidla, například Zašifrovat *všechny zprávy.*
4. V **části Použít toto pravidlo zvolte** **[Použít u všech zpráv]**. 
5. Vedle pole **Provést následující klikněte** na Vybrat jednu z **nich.** 
6. V rozevírací **nabídce šablony RMS** vyberte **Šifrovat** a potom klikněte na **OK.** (Pokud tuto možnost nevidíte, znamená to, že váš plán nezahrnuje automatické šifrování. Můžete ho ale přidat!)
7. Zaškrtněte políčko **Auditovat toto pravidlo s** úrovní závažnosti a vyberte požadovanou úroveň. Pokud má vaše společnost smluvní povinnosti, aby se odesílali všechny e-maily zašifrované, doporučujeme nastavit úroveň **na Vysokou.**
8. V **části Zvolte model pro toto pravidlo** klikněte na **Vynutit.** 
9. Zvolte libovolný volitelný výběr (ze seznamu volitelných výběrů, které můžete v tomto okamžiku provést, z nichž mnohé mohou být ponechány s výchozím nastavením pro jednoduchost).
10. Klikněte na **Uložit**.

> [!IMPORTANT]
> Toto pravidlo můžete později zase vrátit a upravit.

Další informace o vytváření pravidel pro šifrování najdete v článku Definice pravidel toku pošty pro šifrování e-mailových zpráv v [Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

