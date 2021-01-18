---
title: Konfigurace proxy aplikací
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884946"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="c7050-102">Konfigurace proxy aplikací</span><span class="sxs-lookup"><span data-stu-id="c7050-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="c7050-103">Informace o tom, jak nakonfigurovat aplikaci proxy aplikací v rámci Azure AD k vystavení místních aplikací v cloudu, najdete v tématu [jak nakonfigurovat aplikaci proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)aplikace.</span><span class="sxs-lookup"><span data-stu-id="c7050-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="c7050-104">Jednotné přihlašování (SSO) umožňuje uživatelům přistupovat k aplikaci bez nutnosti vícenásobného ověřování.</span><span class="sxs-lookup"><span data-stu-id="c7050-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="c7050-105">Umožňuje jediné ověřování v cloudu – službě Azure Active Directory a umožňuje službě nebo konektoru zosobnit uživatele k provedení dalších výzev k ověření v aplikaci.</span><span class="sxs-lookup"><span data-stu-id="c7050-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="c7050-106">Další informace najdete v tématu [jak nakonfigurovat jednotné přihlašování k aplikaci proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)aplikace.</span><span class="sxs-lookup"><span data-stu-id="c7050-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="c7050-107">[Tento článek](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) se používá k řešení běžných problémů při vytváření nové aplikace proxy aplikace.</span><span class="sxs-lookup"><span data-stu-id="c7050-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="c7050-108">Pokud máte problém s nastavením ověřování back-end pro vaši aplikaci, může být potřeba vyřešit problém [s omezením konfigurace delegování protokolu Kerberos pro proxy aplikace](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) nebo podle pokynů ke [konfiguraci aplikací pomocí PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) .</span><span class="sxs-lookup"><span data-stu-id="c7050-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
