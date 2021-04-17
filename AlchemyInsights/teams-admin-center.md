---
title: Centrum pro správu Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826372"
---
# <a name="teams-admin-center"></a><span data-ttu-id="a4934-102">Centrum pro správu Teams</span><span class="sxs-lookup"><span data-stu-id="a4934-102">Teams Admin Center</span></span>

<span data-ttu-id="a4934-103">Přečtěte si informace o správě Teams pomocí [centra pro správu Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="a4934-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="a4934-104">Pokud nemůžete získat přístup k centru pro správu Teams, zkontrolujte následující položky:</span><span class="sxs-lookup"><span data-stu-id="a4934-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="a4934-105">Zkontrolujte, jestli jste povolili příslušné [IP adresy a adresy URL Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na hraničních zařízeních (bráně firewall atd.) nebo v pravidlech brány firewall na místním počítači.</span><span class="sxs-lookup"><span data-stu-id="a4934-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="a4934-106">Zkontrolujte, jestli přihlašovací jméno, které používáte pro přístup k portálu pro správu Teams, odpovídá vašemu uživatelskému jménu uvedenému na [portálu pro správu Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="a4934-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="a4934-107">Pokud se v centru pro správu Teams neobjevují uživatelé, zkontrolujte následující položky:</span><span class="sxs-lookup"><span data-stu-id="a4934-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="a4934-108">Vytvořili jste v posledních 24 hodinách uživatele nebo přiřazovali licence?</span><span class="sxs-lookup"><span data-stu-id="a4934-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="a4934-109">Než otevřete lístek podpory, počkejte alespoň 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="a4934-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="a4934-110">Ověřte, že jste přiřadili správné licence.</span><span class="sxs-lookup"><span data-stu-id="a4934-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="a4934-111">Pokud máte místní službu Active Directory, ověřte, jestli je hodnota [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) nebo adresy SIP v poli ProxyAddresses v místní službě Active Directory jedinečná a formát odpovídá sip:**Uživatelské** jméno uživatele z Centra pro správu [Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)</span><span class="sxs-lookup"><span data-stu-id="a4934-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="a4934-112">Pokud máte v úmyslu zachovat nasazení Serveru Skypu pro firmy a mít uživatele místně a online: Postupujte podle pokynů v části Nastavení hybridního nasazení přes Teams a **Online Skypu** pro firmy v Ovládacích panelech serveru Skypu pro firmy a přesunutí uživatelů online.</span><span class="sxs-lookup"><span data-stu-id="a4934-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
