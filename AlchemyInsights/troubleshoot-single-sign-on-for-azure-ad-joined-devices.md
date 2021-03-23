---
title: Řešení potíží s jednotným přihlašováním pro zařízení připojená k Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035106"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="31e83-102">Řešení potíží s jednotným přihlašováním pro zařízení připojená k Azure AD</span><span class="sxs-lookup"><span data-stu-id="31e83-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="31e83-103">Pokud máte místní prostředí Active Directory (AD) a chcete se připojit k azure AD počítačům připojeným k doméně AD, můžete to udělat pomocí hybridního připojení k Azure AD.</span><span class="sxs-lookup"><span data-stu-id="31e83-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="31e83-104">[Postupy: Plánování implementace připojení k hybridní](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) službě Azure Active Directory vám poskytne související kroky k implementaci hybridního připojení k Azure AD ve vašem prostředí.</span><span class="sxs-lookup"><span data-stu-id="31e83-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="31e83-105">Další informace najdete v tématu Konfigurace zařízení připojených [ke službě Azure AD](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)pro místní Single-Sign v systému Windows Hello pro firmy .</span><span class="sxs-lookup"><span data-stu-id="31e83-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="31e83-106">**Problémy s tokenem primární aktualizace (PRT)**</span><span class="sxs-lookup"><span data-stu-id="31e83-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="31e83-107">Token primární aktualizace (PRT) je klíčový artefakt ověřování Azure AD ve Windows 10, Windows Serveru 2016 a novějších verzích, zařízeních s iOS a Androidem.</span><span class="sxs-lookup"><span data-stu-id="31e83-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="31e83-108">Jedná se o webový token JSON (JWT), který je speciálně vydaný zprostředkovatelům tokenů první strany Microsoftu, aby umožnil jednotné přihlašování (SSO) v aplikacích používaných na těchto zařízeních.</span><span class="sxs-lookup"><span data-stu-id="31e83-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="31e83-109">Podrobnosti o tom, jak se prt vydává, používá a chrání na zařízeních s Windows 10, najdete v tématu Co je token [primární aktualizace?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="31e83-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="31e83-110">**WamDefaultSet: ANO a AzureADPrt: ANO**</span><span class="sxs-lookup"><span data-stu-id="31e83-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="31e83-111">Tato pole označují, jestli se uživatel při přihlášení k zařízení úspěšně ověřil ve službě Azure AD.</span><span class="sxs-lookup"><span data-stu-id="31e83-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="31e83-112">Pokud jsou hodnoty **NE,** může to být kvůli:</span><span class="sxs-lookup"><span data-stu-id="31e83-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="31e83-113">Chybný klíč úložiště v čipu TPM přidruženém k zařízení při registraci (při spouštění zvýšených oprávnění zkontrolujte KeySignTest)</span><span class="sxs-lookup"><span data-stu-id="31e83-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="31e83-114">Alternativní přihlašovací ID</span><span class="sxs-lookup"><span data-stu-id="31e83-114">Alternate Login ID</span></span>
- <span data-ttu-id="31e83-115">Http Proxy nebyl nalezen.</span><span class="sxs-lookup"><span data-stu-id="31e83-115">HTTP Proxy not found</span></span>

<span data-ttu-id="31e83-116">Informace o řešení potíží se zařízeními pomocí příkazu dsregcmd najdete v tématu [Stav jednotného přihlašování](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="31e83-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
