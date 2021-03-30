---
title: Single-Sign pro zařízení připojená k Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404362"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="5cc7f-102">Jednotné přihlašování pro zařízení připojená k Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="5cc7f-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="5cc7f-103">Pokud máte místní prostředí Active Directory (AD) a chcete se připojit k azure AD počítačům připojeným k doméně AD, můžete to udělat pomocí hybridního připojení k Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5cc7f-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="5cc7f-104">[Postupy: Plánování implementace připojení k hybridní](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) službě Azure Active Directory vám poskytne související kroky k implementaci hybridního připojení k Azure AD ve vašem prostředí.</span><span class="sxs-lookup"><span data-stu-id="5cc7f-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="5cc7f-105">Konfigurace zařízení připojených ke službě Azure AD pro místní Single-Sign v systému Windows Hello pro firmy</span><span class="sxs-lookup"><span data-stu-id="5cc7f-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="5cc7f-106">**Problémy s tokenem primární aktualizace (PRT)** Token primární aktualizace (PRT) je klíčový artefakt ověřování Azure AD ve Windows 10, Windows Serveru 2016 a novějších verzích, zařízeních s iOS a Androidem.</span><span class="sxs-lookup"><span data-stu-id="5cc7f-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="5cc7f-107">Jedná se o webový token JSON (JWT), který je speciálně vydaný zprostředkovatelům tokenů první strany Microsoftu, aby umožnil jednotné přihlašování (SSO) v aplikacích používaných na těchto zařízeních.</span><span class="sxs-lookup"><span data-stu-id="5cc7f-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="5cc7f-108">[V části Co je](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)token primární aktualizace? poskytneme podrobnosti o tom, jak se na zařízeních s Windows 10 vydává, používá a chrání PRT.</span><span class="sxs-lookup"><span data-stu-id="5cc7f-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="5cc7f-109">**WamDefaultSet: ANO a AzureADPrt: ANO** Tato pole označují, jestli se uživatel při přihlášení k zařízení úspěšně ověřil ve službě Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5cc7f-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="5cc7f-110">Pokud jsou hodnoty **NE,** může to být splatné:</span><span class="sxs-lookup"><span data-stu-id="5cc7f-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="5cc7f-111">Chybný klíč úložiště v čipu TPM přidruženém k zařízení při registraci (při spouštění zvýšených oprávnění zkontrolujte KeySignTest).</span><span class="sxs-lookup"><span data-stu-id="5cc7f-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="5cc7f-112">Alternativní přihlašovací ID</span><span class="sxs-lookup"><span data-stu-id="5cc7f-112">Alternate Login ID</span></span>
- <span data-ttu-id="5cc7f-113">Http Proxy nebyl nalezen.</span><span class="sxs-lookup"><span data-stu-id="5cc7f-113">HTTP Proxy not found</span></span>

<span data-ttu-id="5cc7f-114">Poradce při potížích se zařízeními pomocí příkazu dsregcmd – [stav jednotného přihlašování](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="5cc7f-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
