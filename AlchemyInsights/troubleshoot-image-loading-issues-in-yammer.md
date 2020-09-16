---
title: Řešení problémů s načítáním obrázku v Yammeru
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
- "6000"
- "9003112"
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690236"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="79e87-102">Řešení problémů s načítáním obrázku v Yammeru</span><span class="sxs-lookup"><span data-stu-id="79e87-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="79e87-103">Když se v Yammeru vyskytnou problémy s náhledy fotek a souborů, zkuste problém vyřešit tak, že zkontrolujete, jestli k problému dochází u všech uživatelů, jestli k němu dojde na mobilních zařízeních, a jestli je při nahrání přílohy reprodukovatelná.</span><span class="sxs-lookup"><span data-stu-id="79e87-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="79e87-104">**Problémy s fotkou profilu**</span><span class="sxs-lookup"><span data-stu-id="79e87-104">**Profile photo issues**</span></span>  

<span data-ttu-id="79e87-105">Pokud se koncoví uživatelé přihlásí do služby Yammer přes Microsoft 365, musí změnit profil, včetně fotografie profilu.</span><span class="sxs-lookup"><span data-stu-id="79e87-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="79e87-106">Pokud uživatelé nemají oprávnění k aktualizaci profilu, může správce tuto aktualizaci učinit.</span><span class="sxs-lookup"><span data-stu-id="79e87-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="79e87-107">Další informace najdete v článku [zobrazení a aktualizace profilu v Office Delvu](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="79e87-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="79e87-108">Informace o úpravách profilů, včetně fotografií profilu, najdete v tématu [Změna profilu a nastavení Yammeru](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="79e87-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="79e87-109">Aktualizované fotografie profilu se synchronizují jinak než atributy profilu.</span><span class="sxs-lookup"><span data-stu-id="79e87-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="79e87-110">Uživatelé se musí přihlásit, abyste mohli zahájit synchronizaci své fotky profilu.</span><span class="sxs-lookup"><span data-stu-id="79e87-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="79e87-111">Informace najdete v tématu [obrázky profilů uživatelů aktualizované z Office 365 na Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="79e87-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="79e87-112">Informace o životním cyklu uživatele pro Yammer najdete v tématu [Správa uživatelů Yammeru napříč životním cyklem z Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="79e87-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="79e87-113">Podrobnosti o tom, jak synchronizace obrázků v profilu funguje v Microsoft 365, najdete v tématu [informace o synchronizaci profilů obrázků v microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="79e87-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="79e87-114">**Problémy s náhledy dokumentů a miniaturami obrázků**</span><span class="sxs-lookup"><span data-stu-id="79e87-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="79e87-115">Když se do Yammeru zaúčtují soubory nebo obrázky, nemusí se zobrazit náhledy z těchto důvodů:</span><span class="sxs-lookup"><span data-stu-id="79e87-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="79e87-116">Soubor je poškozený a nedá se zpracovat.</span><span class="sxs-lookup"><span data-stu-id="79e87-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="79e87-117">Soubor nebyl nedávno nahrán v SharePointu Online nebo Yammer nemá platná metadata z jiných důvodů.</span><span class="sxs-lookup"><span data-stu-id="79e87-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="79e87-118">Adresy URL potřebné k načtení obrázků náhledu jsou blokovány.</span><span class="sxs-lookup"><span data-stu-id="79e87-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="79e87-119">Náhled souboru byl před odesláním odebrán uživatelem.</span><span class="sxs-lookup"><span data-stu-id="79e87-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="79e87-120">Chyba služby zabránila vygenerování náhledu.</span><span class="sxs-lookup"><span data-stu-id="79e87-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="79e87-121">**Poznámka:** Náhledy odkazů a odesílání souborů se můžou chovat jinak.</span><span class="sxs-lookup"><span data-stu-id="79e87-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="79e87-122">Odkazy na soubory na internetu nebo odkazy, které vyžadují další ověřování, se nemusí zobrazovat správně.</span><span class="sxs-lookup"><span data-stu-id="79e87-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="79e87-123">Další informace najdete v článku [připojení souboru nebo obrázku ke zprávě Yammeru](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="79e87-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 