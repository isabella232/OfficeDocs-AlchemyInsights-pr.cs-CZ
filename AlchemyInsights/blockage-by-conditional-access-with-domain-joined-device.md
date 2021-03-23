---
title: Zablokuje mě podmíněný přístup pomocí zařízení připojeného k doméně.
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/20/2021
ms.locfileid: "51035724"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="b0812-102">Zablokuje mě podmíněný přístup pomocí zařízení připojeného k doméně.</span><span class="sxs-lookup"><span data-stu-id="b0812-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="b0812-103">**Vysoce doporučené nástroje**</span><span class="sxs-lookup"><span data-stu-id="b0812-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="b0812-104">[Nástroj Poradce při potížích s registrací zařízení](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – nástroj, který pomáhá při řešení nejčastějších problémů s registrací zařízení.</span><span class="sxs-lookup"><span data-stu-id="b0812-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="b0812-105">[Skript Připojení k registraci testovacího zařízení](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – Skript, který pomáhá zajistit, aby zařízení bylo přístup k koncovým bodům registrace zařízení pod systémovým účtem.</span><span class="sxs-lookup"><span data-stu-id="b0812-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="b0812-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) – Skript, který vám umožní vyhledávat a spravovat zastaralá zařízení ve vašem prostředí.</span><span class="sxs-lookup"><span data-stu-id="b0812-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="b0812-107">Tady jsou některé běžné důvody, proč může podmíněný přístup selhávát u zařízení, které se připojilo k doméně (hybridní Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b0812-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="b0812-108">**Na zařízení není žádná služba Azure AD PRT** – musíte zajistit, aby zařízení měl primární obnovovací token (PRT) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b0812-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="b0812-109">Další informace o nástroji PRT najdete v tomto [dokumentu.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="b0812-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="b0812-110">Pokud chcete ověřit, jestli máte Azure AD PRT, můžete na zařízení spustit příkaz a ověřit, jestli `dsregcmd/status` se "AzureAdPrt" rovná "ANO".</span><span class="sxs-lookup"><span data-stu-id="b0812-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="b0812-111">Pokud "AzureAdPrt" je "NE", zkontrolujte následující:</span><span class="sxs-lookup"><span data-stu-id="b0812-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="b0812-112">Ať už máte **federované** prostředí se službou AD FS a není dostupné z domácích sítí uživatelů : V takovém případě zajistěte, aby byly vaše koncové body "usernamemixed" přístupné z extranetu.</span><span class="sxs-lookup"><span data-stu-id="b0812-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="b0812-113">Pokud je služba AD FS za sítí VPN, ujistěte se, že se uživatelé připojují k síti VPN, a znovu se přihlaste k zařízení.</span><span class="sxs-lookup"><span data-stu-id="b0812-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="b0812-114">Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="b0812-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="b0812-115">**Jestli je čip TPM** zařízení vadný, a proto ho nemůže ověřit : Zkontrolujte "tpm.msc", jestli je stav čipu TPM připravený.</span><span class="sxs-lookup"><span data-stu-id="b0812-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="b0812-116">Pokud ne, spusťte `dsregcmd/leave` a nechte zařízení znovu připojit k Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b0812-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="b0812-117">Pak to zkuste znovu.</span><span class="sxs-lookup"><span data-stu-id="b0812-117">Then, try again.</span></span> <span data-ttu-id="b0812-118">Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="b0812-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="b0812-119">Používáte poskytovatele identity třetí **strany, který nepodporuje WS-Trust.**</span><span class="sxs-lookup"><span data-stu-id="b0812-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="b0812-120">Jak je popsáno v našich dokumentech, hybridní zařízení připojená k Azure AD v tomto případě nefungují.</span><span class="sxs-lookup"><span data-stu-id="b0812-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="b0812-121">Pro podporu prosím pracujte se svým poskytovatelem identity.</span><span class="sxs-lookup"><span data-stu-id="b0812-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="b0812-122">Uživatelé používají prohlížeč Chrome bez účtů **Windows 10** nebo rozšíření Office Chrome automaticky nepou ít prt na zařízeních připojených ke službě AAD nebo hybridních zařízeních připojených ke službě **AAD:** To vede k selhání všech zásad podmíněného přístupu založených na zařízení s chybovou zprávou "Neregistrované zařízení".</span><span class="sxs-lookup"><span data-stu-id="b0812-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="b0812-123">Pokud chcete prohlížeč Chrome používat správně, musíte si nainstalovat "Účty Windows 10" nebo "Rozšíření Office pro prohlížeč Chrome uživatelů" přes SCCM nebo Intune.</span><span class="sxs-lookup"><span data-stu-id="b0812-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="b0812-124">Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="b0812-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="b0812-125">Pokud není možné rozšíření vzdáleně posunout, upozorní uživatele, aby si ručně nainstalují jedno z výše uvedených rozšíření pro přístup k aplikacím za podmíněným přístupem založeným na zařízeních.</span><span class="sxs-lookup"><span data-stu-id="b0812-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="b0812-126">Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="b0812-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="b0812-127">Zařízení bylo správně připojeno k Hybridní službě Azure AD, ale neúmyslně se odstranilo nebo zakázal, a to buď kvůli změnám synchronizace v **Azure AD Connect,** nebo z webu Azure Portal : Pokud k tomu dojde, objekt zařízení se už nerozpozná jako plně připojené zařízení, i když se stav "AzureAdJoined" a "PRT" na zařízení zobrazí jako platný.</span><span class="sxs-lookup"><span data-stu-id="b0812-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="b0812-128">Tento problém vyřešíte tak, že spustíte na dotčených zařízeních a umožníte jim znovu připojit `dsregcmd/leave` se k Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b0812-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="b0812-129">Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="b0812-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="b0812-130">Pokud jsou vaše zařízení ve Windows 10, 1809 update, s VPN/Cloud Proxy a zobrazí se problémy se stavem AzureAdPrt nebo libovolnou aplikací s problémem jednotného přihlašování (outlook se ne připojuje k poštovní schránce, i když jste měli PRT), zkontrolujte, jestli máte tuto opravu [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) nebo dubnovou kumulativní aktualizaci [KB4549949,](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) aby se zabránilo selhání PRT na těchto počítačích.</span><span class="sxs-lookup"><span data-stu-id="b0812-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















