---
title: Identifikace událostí odstranit zprávy v protokolech auditování
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7e13c9e5fbfa6ade065c2810150687085c1a9daae1a11c134688ec9a83ad37d9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54115641"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Protokoly auditování odstraněných e-mailových zpráv

Od ledna 2019 microsoft ve výchozím nastavení zahajuje protokolování auditování poštovní schránky. Pokud chcete zkontrolovat události odstranění zprávy pro určitého uživatele, musíte akce odstranění pro auditování povolit ručně. Pokud je protokolování auditování poštovní schránky pro vaši organizaci nebo pro konkrétního uživatele už povolené, postupujte podle následujících pokynů.

1. Přihlaste se do [Centra Microsoft 365 dodržování předpisů](https://protection.office.com/)

2. Klikněte **na Hledat a prošeetření** a vyberte Hledání v protokolu **auditování.**

3. Vyberte rozsah dat v **polích Počáteční datum** a **Koncové** datum. Zadejte uživatelské jméno uživatele, kterého chcete prozkoumat (uživatele, který položky odstranil). V poli **Aktivity** vyberte Odstraněná pošta **ze složky Odstraněná pošta** a Přesunuté zprávy do složky **Odstraněná pošta.**

4. Klikněte na **Hledat.**

Ve výsledcích vyberte záznam auditování. V informačním podokně podrobností klikněte na **Další informace**. Další informace o odstraněné položce (například řádek předmětu a umístění položky při odstranění) se zobrazí v poli **AffectedItems.** Vlastnost **ClientInfoString** se zobrazí, pokud k odstranění došlo v Outlook, Outlook na webu (dříve označované jako Outlook Web App) nebo v jiném zařízení.

Další informace najdete v článku [Určení, kdo nastavil přeposílání e-mailů pro poštovní schránku](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Poznámka:** Pomocí funkce protokolu auditování nemůžete načíst odstraněné položky. Pokud chcete načíst odstraněné zprávy v Outlook na webu, podívejte se na stránku Obnovení odstraněných [položek v Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
