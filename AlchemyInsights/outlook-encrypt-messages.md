---
title: S/MIME v Outlooku na webu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772255"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifrování e-mailových zpráv v Outlooku

Šifrování zpráv Microsoft 365 je postavené na platformě Microsoft Azure Rights Management (Azure RMS), která je součástí Azure Information Protection. Pokud vaše předplatné obsahuje Azure Rights Management nebo Azure Information Protection, **nemusíte provádět žádné akce pro ruční povolení nebo aktivaci** služby Rights Management.

V závislosti na názorech zákazníků už nebudete moct povolit automatické šifrování odchozích e-mailů s určitým typem citlivých informací ve vašem tenantovi ve výchozím nastavení. Místo toho nabízíme podrobné pokyny, jak to yourselves. Další podrobnosti o tom, jak vytvořit pravidlo přenosu pro šifrování citlivých informací, najdete v [tomto článku](https://aka.ms/OmeEtr).

- Pokud používáte Outlook na webu (dřív to byl **OWA**): při vytváření e-mailové zprávy jednoduše klikněte na **chránit** v OWA. Bude použito oprávnění "Nepředávat dál". Klikněte na **změnit oprávnění** a zvolte **zašifrovat** , abyste zprávu zašifroval jenom.

- Pokud používáte **klienta Outlooku**: Pokud chcete poslat šifrovanou zprávu z Outlook 2013 nebo 2016 nebo Outlooku 2016 pro Mac, vyberte **Možnosti**  >  **oprávnění**a pak vyberte požadovanou možnost ochrany.

- Chcete **-li automaticky zašifrovat všechny e-maily** poslané určitým příjemcům nebo organizacím externích partnerů, musíte v centru pro správu Exchange vytvořit pravidlo přenosu pošty. Podrobné pokyny [najdete v tomto článku podpory](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

