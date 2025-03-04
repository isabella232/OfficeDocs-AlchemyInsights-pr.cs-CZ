---
title: Vyhledání IP adresy v protokolu auditování
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902253"
---
# <a name="find-the-ip-address-in-audit-log"></a>Vyhledání IP adresy v protokolu auditování

IP adresa, která odpovídá aktivitě prováděné uživatelem nebo správcem, se zobrazuje v protokolech auditování. Zaprotokoluje se taky informace o klientovi. Tady je postup, jak identifikovat IP adresu:

1. Proveďte jednu z následujících akcí:
   - V Centrum dodržování předpisů Microsoftu 365 přejděte <https://compliance.microsoft.com> na **Audit** \> **řešení**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://compliance.microsoft.com/auditlogsearch> .
   - Na portálu Microsoft 365 Defender přejděte <https://security.microsoft.com> na **Audit**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Pokud se zobrazí oznámení, že je potřeba auditování zapnout, pokračujte a zapněte ho hned. Pokud tato funkce není povolená, výsledky hledání nebudou moct natahovat data z předchozích dat.

2. Na stránce **Auditování** ověřte, že **je vybraná karta** Hledání, a nakonfigurujte následující nastavení:
   - **Rozsah dat a času:** V polích  Začátek a **Konec** vyberte rozsah dat a času.
   - **Aktivity:** Pokud vás zajímá určitá aktivita, vyberte ji ze seznamu. v opačném případě se vrátí výchozí hodnota Zobrazit výsledky pro **všechny** aktivity. Všimněte si, že některé aktivity nemusí být dostupné pro výběr. Pokud je však vybrána možnost Zobrazit výsledky **pro všechny** aktivity, budou tyto položky auditování vráceny.
   - **Uživatelé:** Přijměte prázdnou výchozí hodnotu, aby se vrátily výsledky pro všechny uživatele, nebo zadejte jednoho nebo více uživatelů.

3. Až skončíte, klikněte na **Hledat**. Aktivity se zobrazí na nové stránce **vyhledávání auditování.**

4. Ve výsledcích klikněte na **Filtrovat výsledky** **a** do pole filtru aktivity zadejte Nastavit poštovní schránku.

5. Výběrem záznamu auditování ve výsledcích otevřete plovoucí **okno Podrobnosti.**

Další informace najdete v tématu Hledání v protokolu auditování a [prošetřování běžných problémů s podporou](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
