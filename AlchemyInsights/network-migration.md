---
title: Migrace sítě
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "716"
- "6000002"
ms.assetid: b5ab885c-3803-4cc8-adab-94848e226ffb
ms.openlocfilehash: 6f026f932bb35d12d32ce7eddf49e49a44db7f31
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799557"
---
# <a name="network-migration"></a><span data-ttu-id="37cce-102">Migrace sítě</span><span class="sxs-lookup"><span data-stu-id="37cce-102">Network Migration</span></span>

<span data-ttu-id="37cce-103">Váš tenant v O365 je možná přidružený k více sítím Yammer v rámci 1 tenanta: mnoho konfigurací sítí.</span><span class="sxs-lookup"><span data-stu-id="37cce-103">Your O365 tenant is possibly associated with multiple Yammer networks in a 1 tenant : Many networks configuration.</span></span> <span data-ttu-id="37cce-104">Začínáte 16. října 2018, Yammer už nepodporuje víc sítí Yammer přidružených k jednomu tenantovi.</span><span class="sxs-lookup"><span data-stu-id="37cce-104">Starting October 16, 2018, Yammer will no longer support multiple Yammer networks associated with one tenant.</span></span> <span data-ttu-id="37cce-105">Pomocí migrace sítě můžete získat přístup k preferované konfiguraci 1:1.</span><span class="sxs-lookup"><span data-stu-id="37cce-105">You can perform a Network Migration to get to a preferred 1:1 configuration.</span></span>
  
- <span data-ttu-id="37cce-106">Pokud chcete zobrazit seznam sítí přidružených k vašemu tenantovi, přihlaste se ke službě Yammer jako globální správce a přejděte na **správce sítě**a pak klikněte na **migrace sítě**.</span><span class="sxs-lookup"><span data-stu-id="37cce-106">To view a list of the networks associated with your tenant, log in to Yammer as an Global Administrator and browse to **Network Admin**, then **Network Migration**.</span></span> <span data-ttu-id="37cce-107">Zvolte **Další**.</span><span class="sxs-lookup"><span data-stu-id="37cce-107">Choose **Next**.</span></span>

- <span data-ttu-id="37cce-108">Pokud vidíte více sítí uvedených v kroku 2 ze 3, máte k tenantovi O365 přidruženou více sítí Yammer.</span><span class="sxs-lookup"><span data-stu-id="37cce-108">If you see multiple networks listed on Step 2 of 3, then you have multiple Yammer networks associated with your O365 tenant.</span></span>

- <span data-ttu-id="37cce-109">Pokud chcete opravit konfiguraci pro konfiguraci 1:1, pokračujte pomocí nástroje pro migraci sítě.</span><span class="sxs-lookup"><span data-stu-id="37cce-109">To correct your configuration to a 1:1 configuration, continue using the Network Migration tool.</span></span>

- <span data-ttu-id="37cce-110">Další informace o migraci sítě najdete v článku [migrace sítě: Konsolidujte více sítí Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="37cce-110">For more information on Network Migration please see [Network migration: Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

<span data-ttu-id="37cce-111">Poznámka:</span><span class="sxs-lookup"><span data-stu-id="37cce-111">Please Note:</span></span>
  
- <span data-ttu-id="37cce-112">**Migrace sítě migruje jenom aktivní a čekající uživatele.**</span><span class="sxs-lookup"><span data-stu-id="37cce-112">**A network migration migrates only the active and pending users.**</span></span> <span data-ttu-id="37cce-113">Spolu s aktivními uživateli jsou také přeneseny i informace o uživatelích, například jméno a profilový obrázek.</span><span class="sxs-lookup"><span data-stu-id="37cce-113">Along with the active users, the users' information, such as name and profile picture, is also migrated.</span></span> <span data-ttu-id="37cce-114">Žádný obsah sítě, včetně skupin, není migrován.</span><span class="sxs-lookup"><span data-stu-id="37cce-114">Any network content, including groups, is not migrated.</span></span>

- <span data-ttu-id="37cce-115">**Migrace sítě nemůže být stornována.**</span><span class="sxs-lookup"><span data-stu-id="37cce-115">**Network migration can't be reversed.**</span></span> <span data-ttu-id="37cce-116">Po migraci nebudete mít přístup k místní síti ani jejímu obsahu.</span><span class="sxs-lookup"><span data-stu-id="37cce-116">You will not be able to access your subsidiary network and its content after migration.</span></span> <span data-ttu-id="37cce-117">Ještě před tím, než zvažte migraci, chcete pečlivě naplánovat.</span><span class="sxs-lookup"><span data-stu-id="37cce-117">So before you consider a migration, you want to plan carefully.</span></span>
