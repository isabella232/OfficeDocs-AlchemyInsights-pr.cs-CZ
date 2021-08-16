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
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030751"
---
# <a name="do-site-discovery"></a>Zjišťování webů

Pokud vaše organizace stále používá starší webové aplikace a plány k použití režimu Internet Exploreru (což většina zákazníků používá), měli byste udělat nějaké další zjišťování webu.

**Už jste nasadili starší verzi Microsoft Edge**

Pokud jste už svůj seznam webů Enterprise nakonfigurovali tak, aby fungoval pro starší verzi Microsoft Edge, je zjišťování webu téměř hotové. Možná budete muset přidat neutrální weby.

Neutrální weby jsou obvykle weby, které poskytují jednotné přihlašování (SSO). Pokud na neutrální web z Microsoft Edge, chcete zůstat v Microsoft Edge ověření. Pokud v režimu Internet Exploreru přechádíte neutrální web, chcete zůstat v režimu Internet Exploreru a ověřit ho.

Identifikujte jakékoli jednotné přihlašování nebo jiné neutrální weby, které používáte, a přidejte je do Enterprise webu.

**Internet Explorer je výchozí prohlížeč.**

Pokud teď používáte jenom Internet Explorer, možná nevíte, které weby upgradují na moderní webové standardy a které internet Explorer pořád vyžadují. Tyto weby budete chtít najít a přidat do Enterprise webu, abyste mohli používat režim Internet Exploreru jenom pro tyto weby.

> [!NOTE]
> [Enterprise zjišťování webů](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) zjistí weby, které můžou potřebovat režim Internet Exploreru. Může shromažďovat data v počítačích Windows Internet Exploreru 8 až Internet Exploreru 11 v Windows 10, Windows 8.1 nebo Windows 7.

**Analýza dat**

Po shromažďování dat webu doporučujeme k analýze dat použít následující čtyřkrokový proces:
1. Data seřadí podle domény a potom podle adresy URL.
2. Definujte hranice aplikace pro konfiguraci režimu Internet Exploreru. Chcete zahrnout všechny weby a webové ovládací prvky, které definují aplikaci, ale nechcete zahrnout další weby a ovládací prvky. Některé weby můžou být stejně jednoduché, jako jiné můžou vyžadovat definování více webů a *https://contoso.com/app1* stránek.
3. Otestujte aplikaci a ověřte, že nativně nefunguje. Mnoho webů nabídne moderní obsah, když rozpozná moderní prohlížeč a nabídne starší obsah jenom v případě, že rozpozná Internet Explorer.
4. Přidejte aplikaci do seznamu Enterprise webu, pokud se nepodaří testovat.

> [!NOTE]
> Osvědčeným postupem je seskupit všechny weby, které obsahují aplikaci. Tímto způsobem je při upgradu aplikace jednodušší odebrat celý web z režimu Internet Exploreru a začít pro tuto aplikaci používat moderní prohlížeč.

Až s zjišťováním webů skončíte a data analyzujete, můžete se začít dívat na strategii kanálu.

