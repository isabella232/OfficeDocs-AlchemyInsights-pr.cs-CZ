---
title: Identifikace událostí odstranění zpráv v protokolech auditování
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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696506"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Protokoly auditování odstraněných e-mailových zpráv

Od ledna 2019 společnost Microsoft ve výchozím nastavení zapíná protokolování auditu poštovní schránky. Pokud chcete v opačném případě zkontrolovat odstranění událostí pro konkrétního uživatele, musíte ručně povolit akce odstranění pro auditování. Pokud je protokolování auditu poštovní schránky pro vaši organizaci nebo pro určitého uživatele povolené, postupujte podle následujících kroků.

1. Přihlášení do [centra dodržování předpisů Microsoft 365 Security &](https://protection.office.com/)

2. Klikněte na **Hledat a vyšetřování** a vyberte **Hledat v protokolu auditování**.

3. V polích **Datum zahájení** a **Datum ukončení** vyberte rozsah dat. Zadejte uživatelské jméno, které chcete prozkoumat (uživatel, který položky odstranil). V poli **aktivity** vyberte **odstraněné zprávy ze složky Odstraněná pošta** a **přesunuté zprávy do složky Odstraněná pošta**.

4. Klikněte na **Hledat**.

Ve výsledcích vyberte záznam auditu. V rozevíracím seznamu podrobností klikněte na **Další informace**. Další informace o odstraněné položce (například předmět a umístění položky po jejím odstranění) se zobrazí v poli **AffectedItems** . Vlastnost **ClientInfoString** se zobrazí, pokud v Outlooku, Outlooku na webu (dřív se říká Outlook Web App) nebo jiném zařízení.

Další informace najdete v tématu [určení, kdo nastavil přeposlání e-mailů pro poštovní schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Poznámka**: odstraněné položky nemůžete načíst pomocí funkce protokol auditování. Pokud chcete v Outlooku na webu načíst odstraněné zprávy, přečtěte si článek [obnovení odstraněných položek v Outlook Web Appu](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
