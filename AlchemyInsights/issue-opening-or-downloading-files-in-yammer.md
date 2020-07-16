---
title: Problém s otevíráním nebo stahováním souborů v Yammeru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148204"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="d1c16-102">Problém s otevíráním nebo stahováním souborů v Yammeru</span><span class="sxs-lookup"><span data-stu-id="d1c16-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="d1c16-103">Klasický Yammer podporuje více možností pro nahrávání souborů do zpráv a skupin.</span><span class="sxs-lookup"><span data-stu-id="d1c16-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="d1c16-104">V závislosti na konfiguraci sítě jsou soubory výchozí pro úložiště v SharePointu.</span><span class="sxs-lookup"><span data-stu-id="d1c16-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="d1c16-105">Výběr souborů v novém Yammeru ještě nepodporuje všechny možnosti dostupné v klasickém Yammeru.</span><span class="sxs-lookup"><span data-stu-id="d1c16-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="d1c16-106">Budoucí aktualizace přidá další funkce.</span><span class="sxs-lookup"><span data-stu-id="d1c16-106">A future update will add additional features.</span></span> <span data-ttu-id="d1c16-107">Další informace najdete v [tématu Připojení souboru nebo obrázku k příspěvku konverzace na Yammeru](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="d1c16-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="d1c16-108">**Soubor nelze otevřít ani stáhnout.**</span><span class="sxs-lookup"><span data-stu-id="d1c16-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="d1c16-109">Soubor se může nahrát do Yammeru, ale taky se propojí se souborem v SharePointu Online.</span><span class="sxs-lookup"><span data-stu-id="d1c16-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="d1c16-110">Chcete-li odstranit potíže, musíte nejprve určit umístění souboru.</span><span class="sxs-lookup"><span data-stu-id="d1c16-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="d1c16-111">Pokud byl soubor odeslán do Yammeru, bude mít adresu URL \*.yammer.com.</span><span class="sxs-lookup"><span data-stu-id="d1c16-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="d1c16-112">Ujistěte se, že jsou odblokovány požadované adresy URL a IP adresy.</span><span class="sxs-lookup"><span data-stu-id="d1c16-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="d1c16-113">Další informace najdete v příspěvku blogu [Použití pevně kódovaných IP adres pro Yammer se nedoporučuje](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="d1c16-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="d1c16-114">Zkontrolujte, zda uživatel, který je také globálním správcem, může soubor stáhnout.</span><span class="sxs-lookup"><span data-stu-id="d1c16-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="d1c16-115">Pokud je soubor soukromý, bude pravděpodobně muset použít režim soukromého obsahu.</span><span class="sxs-lookup"><span data-stu-id="d1c16-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="d1c16-116">Další informace najdete v [tématu Sledování soukromého obsahu v Yammeru](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="d1c16-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="d1c16-117">**Hosté a soubory na úrovni Yammeru na úrovni sítě v SharePointu Online**</span><span class="sxs-lookup"><span data-stu-id="d1c16-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="d1c16-118">[Hosté na úrovni sítě v Yammeru](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) nepoužívají Azure AD B2B a jsou interní pro službu Yammer, takže nemají přístup k souborům Yammeru uloženým v SharePointu.</span><span class="sxs-lookup"><span data-stu-id="d1c16-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="d1c16-119">Vytvořte externího uživatele AAD B2B, který má přístup ke knihovnám dokumentů v SharePointu Online pomocí této identity.</span><span class="sxs-lookup"><span data-stu-id="d1c16-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="d1c16-120">Informace o budoucí podpoře hosta Azure AD B2B v Yammeru najdete v tématu [Podpora hostů typu Business-to-business (B2B) ve verzi Yammer Preview – smluvní podmínky a nejčastější dotazy](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="d1c16-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>