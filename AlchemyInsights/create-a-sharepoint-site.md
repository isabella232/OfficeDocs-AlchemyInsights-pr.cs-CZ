---
title: Vytvoření SharePointového webu
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806932"
---
# <a name="create-a-sharepoint-site"></a>Vytvoření SharePointového webu

Vytvářet nebo spravovat weby z [aktivních webů](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) v centru pro správu SharePointu Další informace najdete v tématu [Správa webů v novém centru pro správu SharePointu](https://docs.microsoft.com/sharepoint/manage-site-creation). 

## <a name="tips"></a>Tipy

- Web se stejnou adresou URL existujícího webu **nelze** vytvořit. Pokud jste odstranili web a chcete adresu URL znovu použít, je možné, že odstraněný web na [odstraněných webech](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)pořád existuje. K opětovnému použití adresy URL bude nutné tento web trvale odstranit. Informace o úplném odebrání webu pomocí PowerShellu najdete v příkladu rutiny [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .
- Někteří uživatelé nemusí být schopni vytvořit web. [Viz Správa vytváření webů v SharePointu Online](https://docs.microsoft.com/sharepoint/manage-site-creation).
- Je možné, že se zdá, že se web zablokoval **na delší dobu** . Pokud od prvního vystavení tohoto problému uplynulo více než 24 hodin, protokolujte lístek podpory. V mnoha případech jsme na řešení ještě pracujeme. Dokončete řešení alespoň 24 hodin.
