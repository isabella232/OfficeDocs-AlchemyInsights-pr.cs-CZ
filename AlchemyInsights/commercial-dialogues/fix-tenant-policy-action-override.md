---
title: Oprava zásad tenanta (přepsání akce)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896068"
---
# <a name="fix-tenant-policy-action-override"></a>Oprava zásad tenanta (přepsání akce)

Tato zpráva se týká jedné z vašich zásad ochrany proti spamu. Pokud chcete zkontrolovat zásady, postupujte takto:

1. Na portálu Microsoft 365 Defender v části Zásady přejděte na Zásady & spolupráce & pravidla zásady hrozeb <https://security.microsoft.com/>  \>  \>  \> **Anti-spam.** 

   Pokud chcete přejít přímo na stránku Zásady ochrany **proti spamu,** použijte <https://security.microsoft.com/antispam> .

2. Na **stránce Anti-spam policies** (Zásady ochrany proti spamu) vyberte  zásadu kliknutím na  název zásady (**Typ** je Vlastní zásada ochrany proti spamu nebo Název je zásada příchozí pošty **antispamové pošty (výchozí).**
3. V plovoucím seznamu podrobností, který se zobrazí, **vyberte v** části **Akce** možnost Upravit akce.
4. V části Akce **zprávy** si projděte výroky spamu **,** spamu s vysokou spolehlivostí, phishingu a phishingu s vysokou spolehlivostí a zkontrolujte, jestli jsou vybrané následující hodnoty:  
   - **Přidání záhlaví X**
   - **Předpřipravené předměty s textem**
   - **Přesměrovat zprávu na e-mailovou adresu**
   - **Odstranit zprávu**
   - **Žádná akce**

   Je možné, že standardní nastavení použité **pro** všechny Exchange Online Protection zákazníci zprávu ovlivnili.

Další informace najdete v tématu [Konfigurace zásad ochrany proti spamu v programu EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
