---
title: Workday to AD User Provisioning goes into quarantine state
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036485"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Workday to AD User Provisioning goes into quarantine state

**Zřizování uživatelů služby Workday to AD přejde do stavu karantény a ve službě AD se vytvoří žádní uživatelé.**

Úloha Zřizování uživatelů služby Workday to AD je v karanténě a v protokolech auditování se zobrazují události selhání exportu s chybovou zprávou **Chyba: OperationsError-SvcErr: Došlo k chybě operace. Pro adresářovou službu nebyl nakonfigurovaný žádný nadřízený odkaz. Adresářová služba proto nemůže vydávat odkazy na objekty mimo tuto doménovou strukturu**. Tato chyba se obvykle zobrazuje, pokud není správně nastavená OU kontejneru služby Active Directory nebo pokud existují problémy s mapováním výrazů použitým pro **parentDistinguishedName**.

U překlepů **zaškrtněte** u parametru Výchozí OU pro nové uživatele. Ujistěte se, že zadaná OU už ve vaší službě AD existuje. Pokud v mapování atributů používáte **parentDistinguishedName,** ujistěte se, že se vždy vyhodnotí jako známý kontejner v doméně AD. Zkontrolujte událost Export v protokolech auditování a zobrazte vygenerovanou hodnotu.

Další podrobnosti o konfiguraci pracovního dne pro automatické zřizování najdete v tématu [Kurz:](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)Konfigurace pracovního dne pro automatické zřizování uživatelů .

