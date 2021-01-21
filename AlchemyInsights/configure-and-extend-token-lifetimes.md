---
title: Konfigurace a rozšíření životnosti tokenů
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916731"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="b217f-102">Konfigurace a rozšíření životnosti tokenů</span><span class="sxs-lookup"><span data-stu-id="b217f-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="b217f-103">Můžete zadat dobu života tokenu Accessu, SAML nebo ID vystaveného společností Microsoft Identity Platform.</span><span class="sxs-lookup"><span data-stu-id="b217f-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="b217f-104">Životnosti tokenů můžete nastavit pro všechny aplikace ve vaší organizaci, pro víceuživatelské (multi-Organization) aplikaci nebo pro konkrétní instanční objekt ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="b217f-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="b217f-105">Další informace najdete v článku [Konfigurace životnosti tokenů](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="b217f-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="b217f-106">Příklady najdete v [části Příklady konfigurace životnosti tokenů](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="b217f-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="b217f-107">Informace o tom, jak nakonfigurovat životnost a kompatibilitu tokenu v Azure Active Directory B2C (Azure AD B2C), najdete v článku [Konfigurace tokenů v Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="b217f-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="b217f-108">Článek [Konfigurace chování relace v Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) popisuje metody jednotného přihlašování používané v Azure AD B2C a umožňuje zvolit nejvhodnější metodu jednotného přihlašování při konfiguraci zásad.</span><span class="sxs-lookup"><span data-stu-id="b217f-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="b217f-109">**Jak dlouho tokeny vyřešíte? Jak dlouho platí?**</span><span class="sxs-lookup"><span data-stu-id="b217f-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="b217f-110">Životnost tokenů je 1 hodina a životnost relace je 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="b217f-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="b217f-111">To znamená, že pokud se neudělaly žádné žádosti za 24 hodin, budete se muset před žádostí o nový token přihlásit znova.</span><span class="sxs-lookup"><span data-stu-id="b217f-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="b217f-112">Po 30. května 2020 nebude moct žádný nový klient používat konfigurovatelné zásady životnosti tokenů pro konfiguraci a obnovovací tokeny.</span><span class="sxs-lookup"><span data-stu-id="b217f-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="b217f-113">Odmítání proběhne do několika měsíců od toho, což znamená, že přestáváme dodržovat zásady existujících relací a obnovovacích tokenů.</span><span class="sxs-lookup"><span data-stu-id="b217f-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="b217f-114">Životnost tokenů přístupu můžete nakonfigurovat po neplatnosti.</span><span class="sxs-lookup"><span data-stu-id="b217f-114">You can still configure access token lifetimes after the deprecation.</span></span>






