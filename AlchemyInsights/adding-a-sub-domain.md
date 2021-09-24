---
title: Přidání podřízené domény
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506252"
---
# <a name="adding-a-sub-domain"></a>Přidání podřízené domény

Podřízené domény je možné přidat do stejného nebo jiného tenanta, než je nadřazená doména. V obou případech musíte spravovat vlastní nastavení DNS na webu svého registrátora. Pokud jste Microsoftu umožňují spravovat nastavení DNS pomocí záznamů NS nebo jste doménu koupili od Microsoftu, nemůžete přidat subdomény, aniž byste to nejdřív změnili.

Nejdřív přidejte nadřazenou doménu a potom ji přidejte. Pokud je subdoména ve stejném tenantovi, není potřeba žádné další ověření. Pokud přidáváte subdomény do samostatného tenanta, je záznam DNS txt nutný pro ověření vlastnictví před přidáním domény a dalších záznamů DNS pro vybrané služby.

- Pokud chcete přidat doménu nebo subdoménu, postupujte podle pokynů průvodce Přidat doménu [nebo](https://admin.microsoft.com/Adminportal#/Domains/Wizard)přidejte doménu nebo subdoménu ručně tak, že přejdeme na **Nastavení**  >  **domény**  >  **Přidat doménu**.

V případě potřeby:

- Pokud chcete změnit, kdo spravuje nastavení DNS pro existující doménu, přejděte na **Nastavení** Domains (Domény), zaškrtněte políčko vedle domény a pak  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)vyberte Manage DNS (Spravovat **DNS).** V průvodci vyberte **Přidat vlastní záznamy DNS** a dokončete průvodce.
- Pokud chcete přidat podřízené domény do zakoupené domény Microsoftu, převete doménu na jiného registrátora a potom proveďte změnu výše a spravujte vlastní záznamy DNS. Pokyny najdete v článku [Přenos domény z Microsoftu na jiného hostitele](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).
- Pokud se zobrazí chybová zpráva, že vaši doménu už používají jiní členové nebo lidé ve vaší organizaci, budete muset nejdřív převzít tento nespravovaný účet před použitím domény. Pokyny najdete v článku [o převzít nespravovaný adresář jako správce v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
