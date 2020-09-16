---
title: Automatické vyčištění zastaralých zařízení v Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715014"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="b48bc-102">Automatické vyčištění zastaralých zařízení v Intune</span><span class="sxs-lookup"><span data-stu-id="b48bc-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="b48bc-103">Intune umožňuje správci nakonfigurovat časový interval mezi 90 a 270 dny, po kterém se zastaralá zařízení odeberou ze služby.</span><span class="sxs-lookup"><span data-stu-id="b48bc-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="b48bc-104">Toto nastavení je celé v organizaci a jakmile se aktivuje okamžitě.</span><span class="sxs-lookup"><span data-stu-id="b48bc-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="b48bc-105">Všechna zařízení, která nejsou vrácená do serveru Intune po dobu, po kterou se nastavení trvale odstraní.</span><span class="sxs-lookup"><span data-stu-id="b48bc-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="b48bc-106">**Poznámka:** Pro tuto akci čištění jsou způsobilé pouze objekty zařízení MDM.</span><span class="sxs-lookup"><span data-stu-id="b48bc-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="b48bc-107">Pouze objekty zařízení EAS jsou vyloučeny.</span><span class="sxs-lookup"><span data-stu-id="b48bc-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="b48bc-108">Další informace o tom, kdy se zařízení stane opravňujícím k odstranění na základě nastavení čištění zařízení a jeho stavu:</span><span class="sxs-lookup"><span data-stu-id="b48bc-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="b48bc-109">Nastavení: **odstranění zařízení po posledním vrácení se změnami: Ano (určitá hodnota (N) v zadaných dnech)**</span><span class="sxs-lookup"><span data-stu-id="b48bc-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="b48bc-110">V závislosti na hodnotě (N), která je v nastavení nakonfigurovaná, služba Intune odstraní zařízení v zadaných dnech od posledního úspěšného ověření.</span><span class="sxs-lookup"><span data-stu-id="b48bc-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="b48bc-111">Nastavení:  **odstranění zařízení po posledním vrácení se změnami: ne**</span><span class="sxs-lookup"><span data-stu-id="b48bc-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="b48bc-112">180 dnů po vypršení platnosti certifikátu zařízení se odstraní.</span><span class="sxs-lookup"><span data-stu-id="b48bc-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="b48bc-113">**Poznámka:** V obou případech je nutné zařízení úspěšně zaregistrovat v Intune.</span><span class="sxs-lookup"><span data-stu-id="b48bc-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="b48bc-114">Registrace proběhne v průběhu prvního vrácení se změnami zařízení se službou Intune.</span><span class="sxs-lookup"><span data-stu-id="b48bc-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="b48bc-115">Pokud se zařízení úspěšně zaregistruje do Intune, ale nezobrazuje se jako registrace, odstraní se zařízení 270 dní po zápisu.</span><span class="sxs-lookup"><span data-stu-id="b48bc-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="b48bc-116">(90 dnů pro označení zařízení jako odvolaného a další 180 dní, než se záznam odstraní.)</span><span class="sxs-lookup"><span data-stu-id="b48bc-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="b48bc-117">V konzole Intune momentálně neexistuje žádný mechanismus pro určení data vypršení platnosti certifikace zařízení pro dané zařízení.</span><span class="sxs-lookup"><span data-stu-id="b48bc-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>