---
title: Vystavení otevírání nebo stahování souborů v Yammeru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695642"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="81953-102">Vystavení otevírání nebo stahování souborů v Yammeru</span><span class="sxs-lookup"><span data-stu-id="81953-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="81953-103">Klasická Yammer podporuje více možností odesílání souborů do zpráv a skupin.</span><span class="sxs-lookup"><span data-stu-id="81953-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="81953-104">V závislosti na konfiguraci sítě se jedná o výchozí nastavení souborů úložiště v SharePointu.</span><span class="sxs-lookup"><span data-stu-id="81953-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="81953-105">Výběr souborů v nové Yammeru zatím nepodporuje všechny možnosti dostupné v klasické Yammeru.</span><span class="sxs-lookup"><span data-stu-id="81953-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="81953-106">Budoucí aktualizace přidá další funkce.</span><span class="sxs-lookup"><span data-stu-id="81953-106">A future update will add additional features.</span></span> <span data-ttu-id="81953-107">Další informace najdete v článku [připojení souboru nebo obrázku ke příspěvku v konverzaci Yammeru](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="81953-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="81953-108">**Soubor nelze otevřít ani stáhnout**</span><span class="sxs-lookup"><span data-stu-id="81953-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="81953-109">Soubor se může nahrát do Yammeru, ale taky se odkazuje na soubor v SharePointu Online.</span><span class="sxs-lookup"><span data-stu-id="81953-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="81953-110">Abyste mohli řešit potíže, musíte nejdřív určit umístění souboru.</span><span class="sxs-lookup"><span data-stu-id="81953-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="81953-111">Pokud se soubor nahrál na Yammer, bude mít adresu URL \*. yammer.com.</span><span class="sxs-lookup"><span data-stu-id="81953-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="81953-112">Zajistěte, aby se odblokovaly požadované adresy URL a IP adresy.</span><span class="sxs-lookup"><span data-stu-id="81953-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="81953-113">Další informace najdete v článku příspěvek na blog [s použitím pevných kódovaných IP adres pro Yammer se nedoporučuje](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="81953-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="81953-114">Zkontrolujte, jestli soubor stáhne uživatel, který je taky globálním správcem.</span><span class="sxs-lookup"><span data-stu-id="81953-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="81953-115">Pokud je soubor soukromý, bude možná potřeba použít režim soukromého obsahu.</span><span class="sxs-lookup"><span data-stu-id="81953-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="81953-116">Další informace najdete [v tématu sledování soukromého obsahu v Yammeru](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="81953-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="81953-117">**Hosté a soubory uživatelů Yammeru na úrovni sítě v SharePointu Online**</span><span class="sxs-lookup"><span data-stu-id="81953-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="81953-118">[Hosté na úrovni sítě v Yammeru](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) nepoužívají Azure AD B2B a jsou vnitřní pro službu Yammer, takže nemají přístup k souborům Yammeru uloženým na SharePointu.</span><span class="sxs-lookup"><span data-stu-id="81953-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="81953-119">Pomocí této identity můžete vytvořit externího uživatele AAD, který má přístup ke knihovnám dokumentů v SharePointu Online.</span><span class="sxs-lookup"><span data-stu-id="81953-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="81953-120">Informace o budoucí podpoře hostů služby Azure AD B2B v Yammeru najdete v článku [Podpora hostů mezi podniky (B2B) v části s informacemi o zákaznících a nejčastější dotazy](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="81953-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>