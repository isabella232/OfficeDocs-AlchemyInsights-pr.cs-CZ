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
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="7bf1e-102">Workday to AD User Provisioning goes into quarantine state</span><span class="sxs-lookup"><span data-stu-id="7bf1e-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="7bf1e-103">**Zřizování uživatelů služby AD v pracovní dny je v karanténě a v ad nejsou vytvořeni žádní uživatelé.**</span><span class="sxs-lookup"><span data-stu-id="7bf1e-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="7bf1e-104">Úloha Workday to AD User Provisioning je v karanténě a protokoly auditování zobrazují události selhání exportu s chybovou zprávou **Chyba: OperationsError-SvcErr: Došlo k chybě operace. Pro adresářovou službu nebyl nakonfigurován žádný nadřízený odkaz. Adresářová služba proto nemůže vydat doporučení** k objektům mimo tuto doménovou strukturu.</span><span class="sxs-lookup"><span data-stu-id="7bf1e-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="7bf1e-105">Tato chyba se obvykle zobrazí, pokud není OU kontejneru služby Active Directory nastaveno správně nebo pokud jsou problémy s mapováním výrazů, které se používají pro **parentDistinguishedName.**</span><span class="sxs-lookup"><span data-stu-id="7bf1e-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="7bf1e-106">Překlepy zkontrolujte u **parametru Výchozí** OU pro nové uživatele.</span><span class="sxs-lookup"><span data-stu-id="7bf1e-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="7bf1e-107">Ujistěte se, že zadaná OU už ve vaší službě AD existuje.</span><span class="sxs-lookup"><span data-stu-id="7bf1e-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="7bf1e-108">Pokud v mapování **atributů používáte parentDistinguishedName,** ujistěte se, že se vždy vyhodnocuje jako známý kontejner v doméně služby AD.</span><span class="sxs-lookup"><span data-stu-id="7bf1e-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="7bf1e-109">Zkontrolujte událost exportu v protokolech auditování a podívejte se na vygenerovanou hodnotu.</span><span class="sxs-lookup"><span data-stu-id="7bf1e-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="7bf1e-110">Další podrobnosti o konfiguraci pracovního dne pro automatické zřizování najdete v kurzu: Konfigurace [funkce Workday pro automatické zřizování uživatelů.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="7bf1e-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

