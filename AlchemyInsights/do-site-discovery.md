---
title: Zjišťování webů
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692670"
---
# <a name="do-site-discovery"></a><span data-ttu-id="79316-102">Zjišťování webů</span><span class="sxs-lookup"><span data-stu-id="79316-102">Do site discovery</span></span>

<span data-ttu-id="79316-103">Pokud vaše organizace pořád používá starší webové aplikace a plány na používání režimu Internet Exploreru (který používá většina zákazníků), měli byste udělat nějaké další zjišťování webů.</span><span class="sxs-lookup"><span data-stu-id="79316-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="79316-104">**Už jste nasadili starší verzi Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="79316-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="79316-105">Pokud jste už seznam podnikového webu nakonfigurovali tak, aby fungoval pro starší verzi Microsoft Edge, je zjišťování webů téměř hotové.</span><span class="sxs-lookup"><span data-stu-id="79316-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="79316-106">Jednu věc, kterou byste měli udělat, je přidat neutrální weby.</span><span class="sxs-lookup"><span data-stu-id="79316-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="79316-107">Neutrální weby jsou obvykle weby, které poskytují jednotné přihlašování (SSO).</span><span class="sxs-lookup"><span data-stu-id="79316-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="79316-108">Pokud z Microsoft Edge přejdeme na neutrální web, pak chcete zůstat v Microsoft Edge a ověřit si ho.</span><span class="sxs-lookup"><span data-stu-id="79316-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="79316-109">Pokud v režimu Internet Exploreru přejděte na neutrální web, chcete ověření zůstat v režimu Internet Exploreru.</span><span class="sxs-lookup"><span data-stu-id="79316-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="79316-110">Identifikujte jakékoli jednotné přihlašování nebo jiné neutrální weby, které používáte, a přidejte je do svého seznamu podnikových webů.</span><span class="sxs-lookup"><span data-stu-id="79316-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="79316-111">**Internet Explorer je váš výchozí prohlížeč.**</span><span class="sxs-lookup"><span data-stu-id="79316-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="79316-112">Pokud teď používáte jenom Internet Explorer, možná nevíte, které weby se upgradují na moderní webové standardy a které internet Explorer pořád vyžadují.</span><span class="sxs-lookup"><span data-stu-id="79316-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="79316-113">Tyto weby budete chtít najít a přidat do seznamu podnikového webu, abyste mohli používat režim Internet Exploreru jenom pro tyto weby.</span><span class="sxs-lookup"><span data-stu-id="79316-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="79316-114">[Zjišťování podnikových](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) webů zjišťuje weby, které můžou potřebovat režim Internet Exploreru.</span><span class="sxs-lookup"><span data-stu-id="79316-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="79316-115">Může shromažďovat data v počítačích s Windows Internet Explorer 8 prostřednictvím Internet Exploreru 11 ve Windows 10, Windows 8.1 nebo Windows 7.</span><span class="sxs-lookup"><span data-stu-id="79316-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="79316-116">**Analýza dat**</span><span class="sxs-lookup"><span data-stu-id="79316-116">**Analyze the data**</span></span>

<span data-ttu-id="79316-117">Po shromažďování dat webu doporučujeme provést analýzu dat pomocí následujících čtyř kroků:</span><span class="sxs-lookup"><span data-stu-id="79316-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="79316-118">Data můžete seřadit podle domény a potom podle adresy URL.</span><span class="sxs-lookup"><span data-stu-id="79316-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="79316-119">Definujte hranice aplikace, které chcete nakonfigurovat pro režim Internet Exploreru.</span><span class="sxs-lookup"><span data-stu-id="79316-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="79316-120">Chcete zahrnout všechny weby a webové ovládací prvky, které definují aplikaci, ale nechcete zahrnout další weby a ovládací prvky.</span><span class="sxs-lookup"><span data-stu-id="79316-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="79316-121">Některé weby můžou být tak jednoduché, jako třeba jiné, ale můžou vyžadovat, abyste *https://contoso.com/app1* definujte několik webů a stránek.</span><span class="sxs-lookup"><span data-stu-id="79316-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="79316-122">Otestujte aplikaci a ověřte, že nefunguje nativně.</span><span class="sxs-lookup"><span data-stu-id="79316-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="79316-123">Hodně webů bude nabízet moderní obsah, když detekují moderní prohlížeč a nabídnou jenom starší obsah při rozpoznání Internet Exploreru.</span><span class="sxs-lookup"><span data-stu-id="79316-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="79316-124">Pokud testování selže, přidejte aplikaci do seznamu podnikových webů.</span><span class="sxs-lookup"><span data-stu-id="79316-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="79316-125">Osvědčený postup je seskupit všechny weby, ze které se skládá aplikace.</span><span class="sxs-lookup"><span data-stu-id="79316-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="79316-126">Díky tomu je jednodušší při upgradu aplikace odebrat z režimu Internet Exploreru celý web a začít pro tuto aplikaci používat moderní prohlížeč.</span><span class="sxs-lookup"><span data-stu-id="79316-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="79316-127">Až hledání webu skončíte a data analyzujete, můžete se začít dívat na strategii kanálu.</span><span class="sxs-lookup"><span data-stu-id="79316-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

