---
title: Automatické vyčištění zastaralých zařízení v Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554836"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="132f8-102">Automatické vyčištění zastaralých zařízení v Intune</span><span class="sxs-lookup"><span data-stu-id="132f8-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="132f8-103">Intune umožňuje správci konfigurovat časový interval mezi 90 a 270 dny, po kterém se ze služby odeberou zastaralá zařízení.</span><span class="sxs-lookup"><span data-stu-id="132f8-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="132f8-104">Toto nastavení je široké pro celou organizaci a po aktivaci vstoupí v platnost okamžitě.</span><span class="sxs-lookup"><span data-stu-id="132f8-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="132f8-105">Všechna zařízení, která nejsou na serveru Intune po dobu přesahující toto nastavení, se trvale odstraní.</span><span class="sxs-lookup"><span data-stu-id="132f8-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="132f8-106">**Poznámka:** Pro tuto akci vyčištění jsou způsobilé pouze objekty zařízení MDM.</span><span class="sxs-lookup"><span data-stu-id="132f8-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="132f8-107">EAS pouze objekty zařízení jsou vyloučeny.</span><span class="sxs-lookup"><span data-stu-id="132f8-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="132f8-108">Další informace o tom, kdy se zařízení stane způsobilým k odstranění na základě nastavení vyčištění zařízení a jeho "stavu":</span><span class="sxs-lookup"><span data-stu-id="132f8-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="132f8-109">Nastavení: **Odstranění zařízení po posledním datu vrácení se změnami: Ano (některé hodnoty (N) ve dnech zadaných)**</span><span class="sxs-lookup"><span data-stu-id="132f8-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="132f8-110">Na základě hodnoty (N) nakonfigurované v nastavení služba Intune odstraní zařízení v určených dnech po posledním úspěšném vrácení se seznámí se se zpět.</span><span class="sxs-lookup"><span data-stu-id="132f8-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="132f8-111">Nastavení: **Odstranění zařízení po posledním datu vrácení se změnami: Ne**</span><span class="sxs-lookup"><span data-stu-id="132f8-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="132f8-112">180 dní po vypršení platnosti certifikátu zařízení a není obnoven, zařízení se odstraní.</span><span class="sxs-lookup"><span data-stu-id="132f8-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="132f8-113">**Poznámka:** V obou případech musí být zařízení úspěšně zaregistrováno v Intune.</span><span class="sxs-lookup"><span data-stu-id="132f8-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="132f8-114">K registraci dojde během prvního vrácení se změnami zařízení se službou Intune.</span><span class="sxs-lookup"><span data-stu-id="132f8-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="132f8-115">Pokud se zařízení úspěšně zaregistruje do Intune, ale neasíduje intune, zařízení se odstraní 270 dní po registraci.</span><span class="sxs-lookup"><span data-stu-id="132f8-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="132f8-116">(90 dní na označení zařízení jako odvolaného a dalších 180 dní na odstranění záznamu.)</span><span class="sxs-lookup"><span data-stu-id="132f8-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="132f8-117">V konzoli Intune momentálně neexistuje žádný mechanismus, který by stanovil datum vypršení platnosti certifikace zařízení pro dané zařízení.</span><span class="sxs-lookup"><span data-stu-id="132f8-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>