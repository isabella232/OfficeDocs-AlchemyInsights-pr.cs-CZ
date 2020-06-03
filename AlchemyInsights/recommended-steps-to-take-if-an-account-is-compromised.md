---
title: Doporučený postup při napadení účtu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "957"
- "3100016"
ms.openlocfilehash: a094862a175184c3ac2a717cc59aefe2470b9fd1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510781"
---
# <a name="recommended-steps-to-take-if-an-account-is-compromised"></a><span data-ttu-id="7892b-102">Doporučený postup při napadení účtu</span><span class="sxs-lookup"><span data-stu-id="7892b-102">Recommended steps to take if an account is compromised</span></span>

[<span data-ttu-id="7892b-103">VIDEO: Oprava napadeného účtu</span><span class="sxs-lookup"><span data-stu-id="7892b-103">VIDEO: Fixing a compromised account</span></span>](https://www.microsoft.com/videoplayer/embed/RE2jvOb?pid=ocpVideo0-innerdiv-oneplayer&amp;postJsllMsg=true&amp;maskLevel=20&amp;autoplay=true)
  
1. <span data-ttu-id="7892b-104">Okamžitě [resetujte uživatelské heslo](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords).</span><span class="sxs-lookup"><span data-stu-id="7892b-104">[Reset the user's password](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords) immediately.</span></span> <span data-ttu-id="7892b-105">Neposílejte koncovému uživateli nové heslo e-mailem.</span><span class="sxs-lookup"><span data-stu-id="7892b-105">Do not communicate the new password through email to the end user.</span></span>

2. <span data-ttu-id="7892b-106">Odeberte všechny podezřelé [adresy pro přeposílání](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding), které jsou nastaveny na úrovni poštovní schránky.</span><span class="sxs-lookup"><span data-stu-id="7892b-106">Remove any suspicious [forwarding addresses](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding) set at the mailbox level.</span></span>

3. <span data-ttu-id="7892b-107">Odeberte všechna podezřelá [pravidla složky Doručená pošta](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED), která jsou v poštovní schránce nastavena.</span><span class="sxs-lookup"><span data-stu-id="7892b-107">Remove any suspicious [inbox rules](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED) set within the mailbox.</span></span>

4. <span data-ttu-id="7892b-108">Pokud má uživatel zablokované posílání e-mailů, [přejděte na stránku Uživatelé s omezením a účet odblokujte](https://protection.office.com/?hash=/restrictedusers).</span><span class="sxs-lookup"><span data-stu-id="7892b-108">If the user is blocked from sending email, [go to the Restricted Users page to unblock the account](https://protection.office.com/?hash=/restrictedusers).</span></span> <span data-ttu-id="7892b-109">Po dokončení by mělo trvat nanejvýš jednu hodinu, než bude uživatel moct pokračovat v odesílání zpráv.</span><span class="sxs-lookup"><span data-stu-id="7892b-109">Once done, the user should be able to resume sending messages within 1 hour.</span></span>

5. <span data-ttu-id="7892b-110">Odeberte účet uživatele z jakýchkoliv [skupin se správní rolí](https://docs.microsoft.com/microsoft-365/admin/add-users/assign-admin-roles) na tak dlouho, dokud nebudete mít jistotu, že už účet není ohrožený.</span><span class="sxs-lookup"><span data-stu-id="7892b-110">Remove the user account from any [administrative role groups](https://docs.microsoft.com/microsoft-365/admin/add-users/assign-admin-roles) until you are confident that the account is no longer compromised.</span></span>

<span data-ttu-id="7892b-111">Abyste minimalizovali možnost úniku dat nebo napadení účtu i v budoucnu, doporučujeme si přečíst článek [o roadmapě zabezpečení Microsoftu 365](https://docs.microsoft.com//office365/securitycompliance/security-roadmap).</span><span class="sxs-lookup"><span data-stu-id="7892b-111">To minimize the potential of a data breach or a compromised account in the future, we recommend reading our [Microsoft 365 security roadmap ](https://docs.microsoft.com//office365/securitycompliance/security-roadmap).</span></span>
  