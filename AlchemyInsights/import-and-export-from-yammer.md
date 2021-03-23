---
title: Import a export z Yammer
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
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035091"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="cc02e-102">Import a export z Yammer</span><span class="sxs-lookup"><span data-stu-id="cc02e-102">Import and export from Yammer</span></span>

<span data-ttu-id="cc02e-103">**Import**</span><span class="sxs-lookup"><span data-stu-id="cc02e-103">**Import**</span></span>

<span data-ttu-id="cc02e-104">Možnosti importu uživatele se liší podle toho, jestli je Yammer v nativním režimu [pro Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)nebo ne.</span><span class="sxs-lookup"><span data-stu-id="cc02e-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="cc02e-105">**Režim,** který není nativní: Uživatele můžete importovat do skupin pomocí možnosti Přidat z adresáře [(omezit](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) na [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) 100 uživatelů) v nastavení skupiny nebo do sítě pomocí hromadné aktualizace v rámci správce sítě.</span><span class="sxs-lookup"><span data-stu-id="cc02e-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="cc02e-106">**Nativní režim:** Operace členství ve skupině a členství v síti by se měly provádět na portálu pro správu [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [na portálu Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)nebo pomocí jiné možnosti Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cc02e-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="cc02e-107">Sítě v nativním režimu už nemají přístup k hromadné aktualizaci a dalším starším funkcím.</span><span class="sxs-lookup"><span data-stu-id="cc02e-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cc02e-108">Yammer import obsahu z správce sítě, i když byla funkce Export dat použitá v jiné síti, nikdy nepodporuje.</span><span class="sxs-lookup"><span data-stu-id="cc02e-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="cc02e-109">Obsah může být znovu publikován partnerskými řešeními nebo rozhraními Yammer REST API.</span><span class="sxs-lookup"><span data-stu-id="cc02e-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="cc02e-110">**Export**</span><span class="sxs-lookup"><span data-stu-id="cc02e-110">**Export**</span></span>

<span data-ttu-id="cc02e-111">[Export síťových dat v rámci](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) správce sítě umožňuje export obsahu z Yammer, včetně zpráv a souborů.</span><span class="sxs-lookup"><span data-stu-id="cc02e-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="cc02e-112">Přílohy mohou být velmi velké a způsobí, že dokončení exportu bude trvat velmi dlouho.</span><span class="sxs-lookup"><span data-stu-id="cc02e-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="cc02e-113">Doporučujeme exportovat aktivní sítě pomocí rozhraní API pro [export](https://developer.yammer.com/docs/data-export-api) dat v kusech po dnech nebo týdnech.</span><span class="sxs-lookup"><span data-stu-id="cc02e-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="cc02e-114">Podpora Microsoftu neposkytuje pro tento účel vlastní skripty.</span><span class="sxs-lookup"><span data-stu-id="cc02e-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="cc02e-115">Existuje samostatný [export GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) pro export obsahu pro jednotlivé uživatele.</span><span class="sxs-lookup"><span data-stu-id="cc02e-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>