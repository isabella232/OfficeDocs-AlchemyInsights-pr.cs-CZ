---
title: Mapování SharePoint knihovny na síťovou jednotku
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 4eae45992d3fe6b31ae4d1aed02484cf20cb2260
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315541"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>Mapování SharePoint knihovny na síťovou jednotku

Místo mapování síťové jednotky synchronizujte soubory SharePoint s novým klientem synchronizační aplikace OneDrivu, který poskytuje soubory na vyžádání. Získejte přístup ke všem souborům na OneDrivu bez použití prostoru místního úložiště. Další informace najdete v tématu Synchronizace [SharePoint a Teams](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) souborů s počítačem a Uložení místa na disku pomocí OneDrive Files [On-Demand pro Windows 10](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e).

Pokud se rozhodnete místo nového klienta synchronizační aplikace OneDrivu [namapovat](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)jednotku, postupujte takto:

- [Řešení potíží s mapovanými síťovými jednotkami, které se připojují k SharePointu Online](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [Chyby ověřování nastanou, když klient nemá podporu TLS 1.2.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**POZNÁMKA:** Pokud používáte Internet Explorer 10 s Windows 8 nebo Windows 7 a při  mapování jednotky  obdržíte přístup odepřen nebo cesta není přístupná, vyřešte tento problém instalací této [opravy hotfix](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d).