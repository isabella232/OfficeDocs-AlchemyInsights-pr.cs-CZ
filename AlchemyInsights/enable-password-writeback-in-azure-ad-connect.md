---
title: Povolení zpětného zápisu hesla ve službě Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: ab4b8692799d08363e1d726f72a3b80dcb598797
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204618"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="21bdf-102">Povolení zpětného zápisu hesla ve službě Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="21bdf-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="21bdf-103">Chcete-li povolit zpětný zápis pro obnovení samoobslužného hesla, nejprve povolte možnost zpětného zápisu ve službě Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="21bdf-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="21bdf-104">Na serveru Azure AD Connect proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="21bdf-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="21bdf-105">Přihlaste se k serveru Azure AD Connect a spusťte průvodce konfigurací **Azure AD Connect.**</span><span class="sxs-lookup"><span data-stu-id="21bdf-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="21bdf-106">Na **úvodní** stránce klepněte na tlačítko **Konfigurovat**.</span><span class="sxs-lookup"><span data-stu-id="21bdf-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="21bdf-107">Na stránce **Další úkoly** vyberte **Přizpůsobit možnosti synchronizace**a klepněte na tlačítko **Další**.</span><span class="sxs-lookup"><span data-stu-id="21bdf-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="21bdf-108">Na stránce **Připojit k Azure AD** zadejte pověření globálního správce pro vašeho klienta Azure a klikněte na Další.</span><span class="sxs-lookup"><span data-stu-id="21bdf-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="21bdf-109">Na stránkách **Connect directories** a **Domain/OU** filtering klepněte na tlačítko **Další**.</span><span class="sxs-lookup"><span data-stu-id="21bdf-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="21bdf-110">Na stránce **Volitelné funkce** zaškrtněte políčko vedle **možnosti Zpětný zápis hesla** a klepněte na tlačítko **Další**.</span><span class="sxs-lookup"><span data-stu-id="21bdf-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="21bdf-111">Na stránce **Připraveno ke konfiguraci** klikněte na **Konfigurovat** a počkejte na dokončení procesu.</span><span class="sxs-lookup"><span data-stu-id="21bdf-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="21bdf-112">Po dokončení konfigurace klepněte na tlačítko **Ukončit**.</span><span class="sxs-lookup"><span data-stu-id="21bdf-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="21bdf-113">Když je ve Službě Azure AD Connect povolen zpětný zápis hesla, nakonfigurujte azure ad ssdr pro zpětný zápis.</span><span class="sxs-lookup"><span data-stu-id="21bdf-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="21bdf-114">Chcete-li povolit zpětný zápis hesla v sspr, proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="21bdf-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="21bdf-115">Přihlaste se k portálu Azure pomocí účtu globálního správce.</span><span class="sxs-lookup"><span data-stu-id="21bdf-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="21bdf-116">Vyhledejte a vyberte **Azure Active Directory**, klikněte na **Obnovit heslo**a pak zvolte Místní **integrace**.</span><span class="sxs-lookup"><span data-stu-id="21bdf-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="21bdf-117">Nastavit možnost **pro zápis hesel do místního adresáře?** **Yes**</span><span class="sxs-lookup"><span data-stu-id="21bdf-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="21bdf-118">Nastavit možnost **Povolit uživatelům odemknout účty bez resetování hesla?** **Yes**</span><span class="sxs-lookup"><span data-stu-id="21bdf-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="21bdf-119">Až budete připraveni, klepněte na tlačítko **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="21bdf-119">When ready, click **Save**.</span></span>

<span data-ttu-id="21bdf-120">Další informace naleznete v tématu [Povolení samoobslužného zpětného zápisu hesla služby Azure Active Directory do místního prostředí](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="21bdf-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>
