---
title: Aktualizace záznamů DNS tak, aby web zůstal u současného poskytovatele hostingu
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007675"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Aktualizace záznamů DNS tak, aby web zůstal u současného poskytovatele hostingu

1. V Centrum pro správu Microsoftu 365 přejděte na stránku Nastavit domény a v seznamu domén vyberte doménu, kterou používáte  >  [](https://admin.microsoft.com/Adminportal#/Domains) pro svůj web.

2. Vyberte **+ Nový vlastní záznam** a zadejte tyto údaje:

  - Pro **Typ DNS** zadejte: **A (adresa)**

  - Jako **Název hostitele nebo alias** zadejte tento symbol: **@**

  - Do pole **IP adresa** zadejte statickou IP adresu, na které je váš web právě hostovaný (třeba 172.16.140.1).

    Je nutné, aby to byla  *statická*  IP adresa webu, ne  *dynamická*  IP adresa. Na serveru, kde je web hostovaný, se ujistěte, že pro svůj veřejný web můžete získat statickou IP adresu.

3. Vyberte **Uložit**.

Kromě toho můžete vytvořit záznam CNAME, který zákazníkům pomůže váš web najít.
  
1. Vyberte **+ Nový vlastní záznam** a zadejte tyto údaje:

  - Pro **Typ DNS** zadejte: **CNAME (alias)**

  - Do **Název hostitele nebo alias** zadejte: **www**

  - Do pole **Ukazatel na adresu** zadejte plně kvalifikovaný název domény pro svůj web (třeba contoso.com).

2. Vyberte **Uložit**.
