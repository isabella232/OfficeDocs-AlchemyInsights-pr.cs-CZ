---
title: Zpětný zápis zařízení
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256701"
---
# <a name="device-writeback"></a><span data-ttu-id="1d73f-102">Zpětný zápis zařízení</span><span class="sxs-lookup"><span data-stu-id="1d73f-102">Device Writeback</span></span>

<span data-ttu-id="1d73f-103">Zpětný zápis zařízení se používá v následujících scénářích:</span><span class="sxs-lookup"><span data-stu-id="1d73f-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="1d73f-104">Povolení [Windows Hello pro firmy pomocí hybridního nasazení důvěryhodnosti certifikátu](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="1d73f-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="1d73f-105">Povolení podmíněného přístupu na základě zařízení pro aplikace chráněné pomocí služby AD FS (2012 R2 nebo vyšší) (ty, které využívají vztahy důvěryhodnosti)</span><span class="sxs-lookup"><span data-stu-id="1d73f-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="1d73f-106">Pro zpětný zápis zařízení je nutné předplatné Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="1d73f-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="1d73f-107">Tím je další zabezpečení a jistotu, že přístup k aplikacím se udělí jenom důvěryhodným zařízením.</span><span class="sxs-lookup"><span data-stu-id="1d73f-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="1d73f-108">Další informace o podmíněném přístupu najdete v tématu Řízení rizik s podmíněným [přístupem](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) a nastavení místního podmíněného přístupu pomocí registrace zařízení Azure [Active Directory.](https://docs.microsoft.com/azure/active-directory/devices/overview)</span><span class="sxs-lookup"><span data-stu-id="1d73f-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="1d73f-109">Další informace o povolení zpětného zápisu zařízení pro zařízení najdete v článku [Povolení zpětného zápisu zařízení.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)</span><span class="sxs-lookup"><span data-stu-id="1d73f-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
