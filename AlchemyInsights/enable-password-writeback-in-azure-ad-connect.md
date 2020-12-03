---
title: Povolení zpětného zápisu hesel v Azure AD Connect
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
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560433"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="3f1ff-102">Povolení zpětného zápisu hesel v Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="3f1ff-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="3f1ff-103">Pokud chcete povolit samoobslužný zápis resetování hesla, nejdřív v Azure AD Connect povolte možnost zpětný zápis.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="3f1ff-104">Ze svého serveru Azure AD Connect udělejte toto:</span><span class="sxs-lookup"><span data-stu-id="3f1ff-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="3f1ff-105">Přihlaste se k serveru Azure AD Connect a spusťte Průvodce konfigurací **Azure AD Connect** .</span><span class="sxs-lookup"><span data-stu-id="3f1ff-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="3f1ff-106">Na **úvodní** stránce klikněte na **Konfigurovat**.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="3f1ff-107">Na stránce **Další úkoly** vyberte **přizpůsobit možnosti synchronizace** a pak klikněte na **Další**.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="3f1ff-108">Na stránce **Connect to Azure AD** zadejte přihlašovací údaje globálního správce pro tenanta Azure a klikněte na **Další**.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="3f1ff-109">Na stránkách **připojit adresáře** a filtrování **domény nebo organizační jednotky** klikněte na **Další**.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="3f1ff-110">Na stránce **volitelné funkce** zaškrtněte políčko u položky **zpětný zápis hesla** a klikněte na **Další**.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="3f1ff-111">Na stránce **připraveno ke konfiguraci** klikněte na **Konfigurovat** a počkejte, až se proces dokončí.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="3f1ff-112">Po dokončení konfigurace klikněte na **konec**.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="3f1ff-113">Když v Azure AD Connect povolíte zpětný zápis hesla, nakonfigurujte Azure AD SSPR pro zpětný zápis.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="3f1ff-114">Pokud chcete povolit zpětný zápis hesel v SSPR, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="3f1ff-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="3f1ff-115">Přihlaste se k portálu Azure pomocí účtu globálního správce.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="3f1ff-116">Vyhledejte a vyberte **Azure Active Directory**, klikněte na **resetovat heslo** a potom klikněte na **Místní integrace**.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="3f1ff-117">Nastavte možnost pro **zápis hesel do místního adresáře?** na **Ano**.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="3f1ff-118">Nastavte možnost **Povolit uživatelům odemknutí účtů, aniž byste museli resetovat heslo?** **Yes**</span><span class="sxs-lookup"><span data-stu-id="3f1ff-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="3f1ff-119">Až budete připraveni, klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-119">When ready, click **Save**.</span></span>

<span data-ttu-id="3f1ff-120">Další informace najdete v tématu [Povolení automatického obnovení hesla služby Azure Active Directory pro místní prostředí](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="3f1ff-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="3f1ff-121">Pokud správce resetuje heslo uživatele na portálu Azure, bude se heslo zapisovat zpátky do místního počítače, pokud je tento uživatel v jeho synchronizaci.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="3f1ff-122">Tato funkce není momentálně podporovaná na portálu pro správu Office.</span><span class="sxs-lookup"><span data-stu-id="3f1ff-122">This functionality is currently not supported in the Office Admin portal.</span></span>