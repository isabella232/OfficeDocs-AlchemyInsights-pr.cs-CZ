---
title: Řešení problémů s hosty
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939372"
---
# <a name="troubleshoot-guest-user-issues"></a>Řešení problémů s hosty

1. Pokyny ke správě přístupu hostů k aplikacím najdete v tématu [Správa přístupu hostů pomocí recenzí přístupu k Azure AD.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. Přidání uživatelů hostů do adresáře na portálu [Azure Portal:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)V tomto rychlém startu přidáte nového uživatele hosta do adresáře Azure AD prostřednictvím portálu Azure Portal, pošlete pozvánku a uvidíte, jak vypadá proces uplatnění pozvánky hosta.
1. [Přidání uživatele hosta pomocí PowerShellu:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)V tomto rychlém startu použijete příkaz New-AzureADMSInvitation pro přidání jednoho hosta do vašeho tenanta Azure.
1. Pokud se chcete dozvědět, jak přiřazovat uživatele a skupiny k podnikovým aplikacím v Azure Active Directory (Azure AD), buď z portálu Azure portal, nebo pomocí PowerShellu, najdete v tématu Správa přiřazení uživatelů pro aplikaci v [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory B2B (Azure AD) spolupracuje s většinou aplikací, které se integrují s Azure AD. V tomto [článku procházíme](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)pokyny pro konfiguraci některých oblíbených aplikací SaaS pro použití s Azure AD B2B.
1. Jako organizace, která využívá funkce spolupráce Azure Active Directory (Azure AD) B2B k pozvání hosta z partnerských organizací do azure AD, teď můžete těmto uživatelům B2B poskytnout přístup k místním aplikacím. Tyto místní aplikace mohou používat ověřování založené na protokolu SAML nebo integrované ověřování Windows ověřování (IWA) s omezeným delegováním Kerberos (KCD). Další informace najdete v tématu [Udělení přístupu uživatelům B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)v Azure AD k místním aplikacím .
1. Zjistěte, [jak udělit místně spravovaným partnerským účtům přístup k cloudovým prostředkům pomocí spolupráce Azure AD B2B.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)