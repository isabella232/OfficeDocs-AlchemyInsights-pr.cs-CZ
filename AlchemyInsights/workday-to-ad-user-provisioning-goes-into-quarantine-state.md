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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481095"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Workday to AD User Provisioning goes into quarantine state

**Zřizování uživatelů služby AD v pracovní dny je v karanténě a v ad nejsou vytvořeni žádní uživatelé.**

Úloha Workday to AD User Provisioning je v karanténě a protokoly auditování zobrazují události selhání exportu s chybovou zprávou **Chyba: OperationsError-SvcErr: Došlo k chybě operace. Pro adresářovou službu nebyl nakonfigurován žádný nadřízený odkaz. Adresářová služba proto nemůže vydat doporučení** k objektům mimo tuto doménovou strukturu. Tato chyba se obvykle zobrazí, pokud není OU kontejneru služby Active Directory nastaveno správně nebo pokud jsou problémy s mapováním výrazů, které se používají pro **parentDistinguishedName.**

Překlepy zkontrolujte u **parametru Výchozí** OU pro nové uživatele. Ujistěte se, že zadaná OU už ve vaší službě AD existuje. Pokud v mapování **atributů používáte parentDistinguishedName,** ujistěte se, že se vždy vyhodnocuje jako známý kontejner v doméně služby AD. Zkontrolujte událost exportu v protokolech auditování a podívejte se na vygenerovanou hodnotu.

Další podrobnosti o konfiguraci pracovního dne pro automatické zřizování najdete v kurzu: Konfigurace [funkce Workday pro automatické zřizování uživatelů.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

