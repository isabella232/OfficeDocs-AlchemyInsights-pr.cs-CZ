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
# <a name="configure-mim-sync-service"></a><span data-ttu-id="a8118-102">Konfigurace synchronizační služby MIM</span><span class="sxs-lookup"><span data-stu-id="a8118-102">Configure MIM Sync service</span></span>

<span data-ttu-id="a8118-103">Synchronizační služba MiM (Microsoft Identity Manager) je součástí mim.</span><span class="sxs-lookup"><span data-stu-id="a8118-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="a8118-104">Jedná se o centralizovanou místní službu, která ukládá a integruje informace pro organizace, které mají více místních adresářů a databází.</span><span class="sxs-lookup"><span data-stu-id="a8118-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="a8118-105">Váš problém se synchronizací MIM Sync můžete vyřešit, pokud byl problém vyřešený v nedávné aktualizaci MIM nebo je to jeden z dalších problémů uvedených v následující části.</span><span class="sxs-lookup"><span data-stu-id="a8118-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="a8118-106">**Doporučené kroky**</span><span class="sxs-lookup"><span data-stu-id="a8118-106">**Recommended steps**</span></span>

1. <span data-ttu-id="a8118-107">Ujistěte se, že používáte nedávnou aktualizaci nástroje MIM Sync, a zkontrolujte poznámky k verzi aplikace [MIM Sync,](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) abyste zjistili, jestli se problém vyřešil v aktualizaci.</span><span class="sxs-lookup"><span data-stu-id="a8118-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="a8118-108">Pokud máte problém s obecným konektorem LDAP, Generic SQL, Lotus Domino nebo Web Services, ujistěte se, že používáte nedávnou aktualizaci [obecných spojnic.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)</span><span class="sxs-lookup"><span data-stu-id="a8118-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="a8118-109">Pokud se při spuštění MIM ukončí s chybou, podívejte se do tabulky kódů chyb, abyste zjistili možné příčiny. [](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes)</span><span class="sxs-lookup"><span data-stu-id="a8118-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="a8118-110">Pokud se spuštění zastaví s výjimkou **přípony dll,** kliknutím  na tato slova otevřete okno vlastností prostoru spojnice a klikněte na Trasování **vrství.** Zobrazí se další informace o příčině, jak je popsáno v tématu Výjimka knihovny [DLL-rozšíření.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)</span><span class="sxs-lookup"><span data-stu-id="a8118-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="a8118-111">Pokud součást služby PCNS (Password Change Notification Service) hlásí chybu **6025** v protokolu událostí během synchronizace hesel, podívejte se do příručky pro řešení potíží s chybou [6025 oznámení PCNS.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)</span><span class="sxs-lookup"><span data-stu-id="a8118-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="a8118-112">Pokud je úplná synchronizace s agentem správy  služeb FIM pomalá, zkontrolujte nastavení automatického růstu pro tempDB, jak je popsáno v části Řešení potíží s pomalou nebo zavěšenou [úplnou synchronizací.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)</span><span class="sxs-lookup"><span data-stu-id="a8118-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="a8118-113">Pokud se setkáte s chybou zastaveno-server s selhal-creation-via-web-services pomocí agenta správy služeb FIM, podívejte se na informace o [podpoře: failed-creation-via-web-services,](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) kde najdete přehled příčin.</span><span class="sxs-lookup"><span data-stu-id="a8118-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

