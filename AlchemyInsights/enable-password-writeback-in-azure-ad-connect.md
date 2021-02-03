---
title: Povolení zpětného zápisu hesla v Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093348"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="2b10d-102">Povolení zpětného zápisu hesla v Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="2b10d-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="2b10d-103">Pokud chcete povolit samoobslužné resetování zápisu hesel, na prvním místě povolte možnost zpětného zápisu v Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="2b10d-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="2b10d-104">Na serveru Azure AD Connect proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="2b10d-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="2b10d-105">Přihlaste se k serveru Azure AD Connect a spusťte **průvodce konfigurací Azure AD Connect.**</span><span class="sxs-lookup"><span data-stu-id="2b10d-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="2b10d-106">Na úvodní **stránce** klikněte na **Konfigurovat.**</span><span class="sxs-lookup"><span data-stu-id="2b10d-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="2b10d-107">Na stránce **Další úkoly** vyberte Přizpůsobit **možnosti synchronizace** a potom klikněte na **Další.**</span><span class="sxs-lookup"><span data-stu-id="2b10d-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="2b10d-108">Na stránce **Připojit k Azure AD** zadejte přihlašovací údaje globálního správce pro vašeho tenanta Azure a klikněte na **Další.**</span><span class="sxs-lookup"><span data-stu-id="2b10d-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="2b10d-109">Na **stránkách připojení adresářů** a filtrování **domény a OU** klikněte na **Další.**</span><span class="sxs-lookup"><span data-stu-id="2b10d-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="2b10d-110">Na stránce **Volitelné funkce** zaškrtněte políčko  vedle možnosti Zpětný zápis hesla a klikněte na **Další.**</span><span class="sxs-lookup"><span data-stu-id="2b10d-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="2b10d-111">Na stránce **Ready to configure** (Připraveno ke konfiguraci) klikněte na **Configure** (Konfigurovat) a počkejte, až proces skončí.</span><span class="sxs-lookup"><span data-stu-id="2b10d-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="2b10d-112">Až uvidíte dokončení konfigurace, klikněte na **Konec.**</span><span class="sxs-lookup"><span data-stu-id="2b10d-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="2b10d-113">Pokud je v Azure AD Connect povolený zpětný zápis hesel, nakonfigurujte Azure AD SSPR pro zpětný zápis.</span><span class="sxs-lookup"><span data-stu-id="2b10d-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="2b10d-114">Pokud chcete v SSPR povolit zpětný zápis hesel, proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="2b10d-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="2b10d-115">Přihlaste se k portálu Azure Portal pomocí účtu globálního správce.</span><span class="sxs-lookup"><span data-stu-id="2b10d-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="2b10d-116">Vyhledejte a vyberte **Azure Active Directory, klikněte** na **Resetování hesla** a potom klikněte na místní **integraci.**</span><span class="sxs-lookup"><span data-stu-id="2b10d-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="2b10d-117">Nastavte možnost pro **zapisování** hesel do místního adresáře? na **Ano.**</span><span class="sxs-lookup"><span data-stu-id="2b10d-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="2b10d-118">Nastavte možnost povolit **uživatelům odemykání účtů bez resetování jejich hesla?** **Nastavte Ano.**</span><span class="sxs-lookup"><span data-stu-id="2b10d-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="2b10d-119">Až budete připravení, klikněte na **Uložit.**</span><span class="sxs-lookup"><span data-stu-id="2b10d-119">When ready, click **Save**.</span></span>

<span data-ttu-id="2b10d-120">Další informace najdete v článku o povolení samoobslužných resetování hesel pro Azure Active Directory do [místního prostředí.](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="2b10d-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="2b10d-121">Když správce resetuje heslo uživatele na portálu Azure Portal a tento uživatel je federovaný nebo synchronizovaný s hodnotou hash hesel, heslo se zapište zpátky do místního prostředí.</span><span class="sxs-lookup"><span data-stu-id="2b10d-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="2b10d-122">Tato funkce vyžaduje licenci Azure Premium (P1 nebo P2) a není momentálně podporovaná na portálu pro správu Office.</span><span class="sxs-lookup"><span data-stu-id="2b10d-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
