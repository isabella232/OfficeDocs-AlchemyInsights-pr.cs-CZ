---
title: Centrum pro správu Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670357"
---
# <a name="teams-admin-center"></a><span data-ttu-id="d5815-102">Centrum pro správu Teams</span><span class="sxs-lookup"><span data-stu-id="d5815-102">Teams Admin Center</span></span>

<span data-ttu-id="d5815-103">Přečtěte si informace o správě Teams pomocí [centra pro správu Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="d5815-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="d5815-104">Pokud nemůžete získat přístup k centru pro správu Teams, zkontrolujte následující položky:</span><span class="sxs-lookup"><span data-stu-id="d5815-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="d5815-105">Zkontrolujte, jestli jste povolili příslušné [IP adresy a adresy URL Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na hraničních zařízeních (bráně firewall atd.) nebo v pravidlech brány firewall na místním počítači.</span><span class="sxs-lookup"><span data-stu-id="d5815-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="d5815-106">Zkontrolujte, jestli přihlašovací jméno, které používáte pro přístup k portálu pro správu Teams, odpovídá vašemu uživatelskému jménu uvedenému na [portálu pro správu Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="d5815-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="d5815-107">Pokud se v centru pro správu Teams neobjevují uživatelé, zkontrolujte následující položky:</span><span class="sxs-lookup"><span data-stu-id="d5815-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="d5815-108">Vytvořili jste v posledních 24 hodinách uživatele nebo přiřazovali licence?</span><span class="sxs-lookup"><span data-stu-id="d5815-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="d5815-109">Než otevřete lístek podpory, počkejte alespoň 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="d5815-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="d5815-110">Ověřte, že jste přiřadili správné licence.</span><span class="sxs-lookup"><span data-stu-id="d5815-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="d5815-111">Pokud máte místní službu Active Directory, ověřte, že [hodnota parametru msRTCSIP-PrimaryUserAddress nebo adresy SIP v poli proxyAddresses v místní službě Active Directory je jedinečná a formát odpovídá](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) protokolu SIP:**uživatelské jméno** uživatele z [centra pro správu Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="d5815-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="d5815-112">Pokud máte v úmyslu zachovat nasazení serveru Skype pro firmy a máte místní i online uživatele, postupujte podle pokynů v **části nastavení hybridu s týmy a Skypu pro firmy** na ovládacím panelu serveru Skype pro firmy a přesunutí uživatelů do online režimu.</span><span class="sxs-lookup"><span data-stu-id="d5815-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
