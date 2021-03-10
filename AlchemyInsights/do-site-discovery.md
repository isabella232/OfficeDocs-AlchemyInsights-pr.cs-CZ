---
title: Zjišťování webů
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692670"
---
# <a name="do-site-discovery"></a>Zjišťování webů

Pokud vaše organizace pořád používá starší webové aplikace a plány na používání režimu Internet Exploreru (který používá většina zákazníků), měli byste udělat nějaké další zjišťování webů.

**Už jste nasadili starší verzi Microsoft Edge**

Pokud jste už seznam podnikového webu nakonfigurovali tak, aby fungoval pro starší verzi Microsoft Edge, je zjišťování webů téměř hotové. Jednu věc, kterou byste měli udělat, je přidat neutrální weby.

Neutrální weby jsou obvykle weby, které poskytují jednotné přihlašování (SSO). Pokud z Microsoft Edge přejdeme na neutrální web, pak chcete zůstat v Microsoft Edge a ověřit si ho. Pokud v režimu Internet Exploreru přejděte na neutrální web, chcete ověření zůstat v režimu Internet Exploreru.

Identifikujte jakékoli jednotné přihlašování nebo jiné neutrální weby, které používáte, a přidejte je do svého seznamu podnikových webů.

**Internet Explorer je váš výchozí prohlížeč.**

Pokud teď používáte jenom Internet Explorer, možná nevíte, které weby se upgradují na moderní webové standardy a které internet Explorer pořád vyžadují. Tyto weby budete chtít najít a přidat do seznamu podnikového webu, abyste mohli používat režim Internet Exploreru jenom pro tyto weby.

> [!NOTE]
> [Zjišťování podnikových](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) webů zjišťuje weby, které můžou potřebovat režim Internet Exploreru. Může shromažďovat data v počítačích s Windows Internet Explorer 8 prostřednictvím Internet Exploreru 11 ve Windows 10, Windows 8.1 nebo Windows 7.

**Analýza dat**

Po shromažďování dat webu doporučujeme provést analýzu dat pomocí následujících čtyř kroků:
1. Data můžete seřadit podle domény a potom podle adresy URL.
2. Definujte hranice aplikace, které chcete nakonfigurovat pro režim Internet Exploreru. Chcete zahrnout všechny weby a webové ovládací prvky, které definují aplikaci, ale nechcete zahrnout další weby a ovládací prvky. Některé weby můžou být tak jednoduché, jako třeba jiné, ale můžou vyžadovat, abyste *https://contoso.com/app1* definujte několik webů a stránek.
3. Otestujte aplikaci a ověřte, že nefunguje nativně. Hodně webů bude nabízet moderní obsah, když detekují moderní prohlížeč a nabídnou jenom starší obsah při rozpoznání Internet Exploreru.
4. Pokud testování selže, přidejte aplikaci do seznamu podnikových webů.

> [!NOTE]
> Osvědčený postup je seskupit všechny weby, ze které se skládá aplikace. Díky tomu je jednodušší při upgradu aplikace odebrat z režimu Internet Exploreru celý web a začít pro tuto aplikaci používat moderní prohlížeč.

Až hledání webu skončíte a data analyzujete, můžete se začít dívat na strategii kanálu.

