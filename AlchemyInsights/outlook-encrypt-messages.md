---
title: S/MIME v Outlook na webu
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
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010717"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifrování e-mailových zpráv v Outlook

Microsoft 365 Šifrování zpráv je postavené na Microsoft Azure Rights Management (Azure RMS), která je součástí Azure Information Protection. Pokud vaše předplatné zahrnuje Azure Rights Management nebo Azure Information Protection, není nutné provádět žádné akce k ručnímu povolení nebo **aktivaci** služby Rights Management Service.

Na základě zpětné vazby od zákazníků už nebudeme povolovat pravidla toku pošty Exchange automaticky šifrovat odchozí e-maily obsahující určitý typ citlivých informací ve vašem tenantovi ve výchozím nastavení. Místo toho poskytujeme podrobné pokyny, jak to můžete udělat sami. Další podrobnosti o tom, jak vytvořit pravidlo přenosu pro šifrování citlivých informací, najdete v [tomto článku.](https://aka.ms/OmeEtr)

- Pokud používáte Outlook na webu (dřív **OWA):** Při vytváření e-mailové zprávy jednoduše klikněte na **Zamknout** v aplikaci OWA. Použije se oprávnění Neposílání dál. Klikněte **na Změnit oprávnění** a zvolte **Šifrovat,** aby se zpráva zašifrovaná jenom zašifruje.

- Pokud používáte klienta **Outlook**: Pokud chcete poslat zašifrovanou zprávu z Outlook 2013 nebo 2016 nebo Outlook 2016 pro Mac, vyberte Možnosti oprávnění a pak vyberte požadovanou možnost   >  ochrany.

- Pokud **chcete automaticky zašifrovat** všechny e-maily odeslané určitým příjemcům nebo externím partnerským organizacím, musíte vytvořit pravidlo přenosu toku pošty v Centru pro správu Exchange pošty. Podrobné pokyny najdete v [tomto článku podpory.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

