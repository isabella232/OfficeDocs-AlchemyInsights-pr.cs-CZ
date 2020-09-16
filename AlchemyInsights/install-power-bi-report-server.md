---
title: Instalace serveru sestav Power BI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1304"
- "2500001"
ms.openlocfilehash: 3ea596547093773ab872ca34e8dd3a4e49e59fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755088"
---
# <a name="install-power-bi-report-server"></a>Instalace serveru sestav Power BI

1. Najděte umístění PowerBIReportServer.exe a spusťte instalační program.

2. Vyberte **nainstalovat server sestav Power BI**.

3. Zvolte edici, kterou chcete nainstalovat, a pak vyberte **Další**.

4. V rozevíracím seznamu můžete zvolit buď hodnocení, nebo edici vývojáře.  Jinak můžete zadat kód Product Key pro server, který jste získali ze služby Power BI nebo služby Volume License Service Center. Další informace o tom, jak získat kód Product Key, najdete v části před začátkem. Čtěte a odsouhlaste s licenčními podmínkami a pak vyberte **Další**.

5. Abyste mohli uložit databázi serveru sestav, musíte mít k dispozici databázový stroj. Výběrem možnosti **Další** nainstalujete pouze Report Server.

6. Zadejte umístění instalace serveru sestav. Pokračujte výběrem možnosti **nainstalovat** .

7. Po úspěšném dokončení instalace vyberte **Konfigurovat server sestav** a spusťte Správce konfigurace služby Reporting Services.

Při instalaci nepotřebujete Server databázového stroje SQL Server dostupný. Po instalaci budete muset nakonfigurovat služby Reporting Services.

Další informace: https://docs.microsoft.com/power-bi/report-server/install-report-server
