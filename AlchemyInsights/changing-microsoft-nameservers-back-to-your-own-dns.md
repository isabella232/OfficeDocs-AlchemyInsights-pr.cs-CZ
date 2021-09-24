---
title: Změna z názvových serverů Microsoftu zpět na správu vlastních záznamů DNS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506385"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Změna z názvových serverů Microsoftu zpět na správu vlastních záznamů DNS

Dříve jste změnili záznamy NS tak, aby odkazly na Microsoft (ns1.bdm.microsoftonline.com), ale teď jste se rozhodli spravovat vlastní záznamy DNS:

Na webu doménového registrátora změňte názvový server zpátky na svého registrátora nebo předchozí nastavení. Jestli se záznamy DNS běžně nepracujete, obraťte se na podporu u svého doménového registrátora. Všimněte si, že šíření změn názvového serveru může trvat až 48 hodin. 

1. Na Microsoft 365 správce přejděte na **Nastavení** Domény , zaškrtněte políčko vedle domény a  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)vyberte **Spravovat DNS**. 

2. V průvodci vyberte **Přidat vlastní záznamy DNS** a dokončete průvodce. Tím změníte způsob, jakým se vaše DNS spravuje, a pak můžete přidat vlastní záznamy DNS potřebné k podpoře vybraných služeb.

Pokud jste změnili záznamy názvových serverů na Microsoft a máte web, můžete místo toho, aby se názvové servery vrátily zpátky, přidat záznamy DNS pro web. Další informace najdete v článku Aktualizace záznamů DNS tak, aby váš web byl u [vašeho současného poskytovatele hostingu](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).


