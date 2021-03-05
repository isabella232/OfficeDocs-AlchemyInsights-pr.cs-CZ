---
title: Konfigurace synchronizační služby MIM
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
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481094"
---
# <a name="configure-mim-sync-service"></a>Konfigurace synchronizační služby MIM

Synchronizační služba MiM (Microsoft Identity Manager) je součástí mim. Jedná se o centralizovanou místní službu, která ukládá a integruje informace pro organizace, které mají více místních adresářů a databází. Váš problém se synchronizací MIM Sync můžete vyřešit, pokud byl problém vyřešený v nedávné aktualizaci MIM nebo je to jeden z dalších problémů uvedených v následující části.

**Doporučené kroky**

1. Ujistěte se, že používáte nedávnou aktualizaci nástroje MIM Sync, a zkontrolujte poznámky k verzi aplikace [MIM Sync,](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) abyste zjistili, jestli se problém vyřešil v aktualizaci.
2. Pokud máte problém s obecným konektorem LDAP, Generic SQL, Lotus Domino nebo Web Services, ujistěte se, že používáte nedávnou aktualizaci [obecných spojnic.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)
3. Pokud se při spuštění MIM ukončí s chybou, podívejte se do tabulky kódů chyb, abyste zjistili možné příčiny. [](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes)
4. Pokud se spuštění zastaví s výjimkou **přípony dll,** kliknutím  na tato slova otevřete okno vlastností prostoru spojnice a klikněte na Trasování **vrství.** Zobrazí se další informace o příčině, jak je popsáno v tématu Výjimka knihovny [DLL-rozšíření.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)
5. Pokud součást služby PCNS (Password Change Notification Service) hlásí chybu **6025** v protokolu událostí během synchronizace hesel, podívejte se do příručky pro řešení potíží s chybou [6025 oznámení PCNS.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)
6. Pokud je úplná synchronizace s agentem správy  služeb FIM pomalá, zkontrolujte nastavení automatického růstu pro tempDB, jak je popsáno v části Řešení potíží s pomalou nebo zavěšenou [úplnou synchronizací.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)
7. Pokud se setkáte s chybou zastaveno-server s selhal-creation-via-web-services pomocí agenta správy služeb FIM, podívejte se na informace o [podpoře: failed-creation-via-web-services,](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) kde najdete přehled příčin.

