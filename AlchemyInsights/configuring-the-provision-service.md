---
title: Konfigurace služby zřizování
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481343"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="bf878-102">Konfigurace služby zřizování</span><span class="sxs-lookup"><span data-stu-id="bf878-102">Configuring the Provision service</span></span>

<span data-ttu-id="bf878-103">Aby automatické zřizování uživatelů fungovalo, vyžaduje Azure AD platné přihlašovací údaje, které mu umožňují připojení k rozhraní API webových služeb Workday.</span><span class="sxs-lookup"><span data-stu-id="bf878-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="bf878-104">Tlačítko Test připojení v pracovním dni dále ověřuje i aplikaci ad User Provisioning, jestli se může připojit k agentovi zřizování Azure AD Connect přidruženému k doméně služby AD.</span><span class="sxs-lookup"><span data-stu-id="bf878-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="bf878-105">Pokud portál Azure Portal při ukládání přihlašovacích údajů vrací chybu, postupujte podle doporučených kroků níže:</span><span class="sxs-lookup"><span data-stu-id="bf878-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="bf878-106">Potvrďte, že jste nakonfigurovali uživatelský účet systému Workday Integration System, jak je uvedeno v oddílu Konfigurace uživatele systému integrace [v pracovním dni.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="bf878-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="bf878-107">Potvrďte, že služba Azure AD Connect Provisioning Agent (Agent Azure AD) je spuštěná na vašem místním serveru Windows pomocí konzoly pro správu služeb.</span><span class="sxs-lookup"><span data-stu-id="bf878-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="bf878-108">Stav agenta můžete zkontrolovat i na portálu Azure Portal kliknutím na tlačítko Zobrazit místní agenty.</span><span class="sxs-lookup"><span data-stu-id="bf878-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="bf878-109">Ujistěte se, že zadáváte hodnotu do pole Workday Username pomocí formátu username@workday-název tenanta.</span><span class="sxs-lookup"><span data-stu-id="bf878-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="bf878-110">Pokud chybí název pracovního dne-tenanta, ověření pracovního dne selže.</span><span class="sxs-lookup"><span data-stu-id="bf878-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="bf878-111">Pokud konfigurujete integraci s tenantem implementace Workday, poznamenejte si naplánovanou pracovní dobu tenanta.</span><span class="sxs-lookup"><span data-stu-id="bf878-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="bf878-112">Pracovní den naplánovat pro tenanty implementace přes víkendy (obvykle od pátečního večera do soboty ráno) a selhání připojení během tohoto intervalu prostoje je známý problém, který se automaticky vyřeší, jakmile tenanti pro implementaci budou zase online.</span><span class="sxs-lookup"><span data-stu-id="bf878-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="bf878-113">Ve výjimečných případech se tato chyba může zobrazit také v případě, že se změnilo heslo uživatele systému integrace kvůli aktualizaci tenanta nebo když je účet uzamčený nebo jeho platnost vypršela.</span><span class="sxs-lookup"><span data-stu-id="bf878-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="bf878-114">Zkontrolujte prosím stav uživatele systému integrace s vaším správcem pracovního dne.</span><span class="sxs-lookup"><span data-stu-id="bf878-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="bf878-115">Další podrobnosti o konfiguraci pracovního dne pro automatické zřizování najdete v kurzu: Konfigurace [funkce Workday pro automatické zřizování uživatelů.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="bf878-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
