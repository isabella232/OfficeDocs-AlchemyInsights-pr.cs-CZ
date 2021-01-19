---
title: Poradce při potížích s uživatelem Host
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900952"
---
# <a name="troubleshoot-guest-user-issues"></a>Poradce při potížích s uživatelem Host

1. Pokyny ke správě přístupu hostů do aplikací najdete v článku [Správa přístupu hostů pomocí kontrol služby Azure AD Access](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Přidání uživatelů typu Host do adresáře na portálu Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): v tomto rychlým automatu přidáte do adresáře Azure AD nového hosta přes Azure Portal, odešlete pozvánku a zjistíte, jak vypadá proces uplatnění pozvání uživatele hosta.
1. [Přidání hostujícího uživatele pomocí PowerShellu](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): v tomto rychlým automatu můžete pomocí příkazu New-AzureADMSInvitation přidat jednoho hostujícího uživatele do tenanta Azure.
1. Informace o tom, jak přiřadit uživatele a skupiny k podnikovým aplikacím v Azure Active Directory (Azure AD), ať už z portálu Azure nebo pomocí PowerShellu, najdete v tématu [Správa přiřazení uživatelů pro aplikaci v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Služba Azure Active Directory (Azure AD) spolupracující spolupráce funguje s většinou aplikací, které se integrují do služby Azure AD. V tomto [článku](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)jsme provedli pokyny pro konfiguraci některých oblíbených aplikací SaaS pro použití se službou Azure AD B2B.
1. Jako organizace, která používá možnosti spolupráce Azure Active Directory (Azure AD) k přizvání uživatelů typu host z partnerských organizací do služby Azure AD, teď můžete těmto uživatelům aplikace B2B umožnit přístup k místním aplikacím. Tyto místní aplikace můžou používat ověřování založené na SAML nebo integrované ověřování systému Windows (IWA) s limitovaným delegováním Kerberos (KCD). Další informace najdete v článku [udělení uživatelů B2B v Azure AD Accessu do místních aplikací](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Zjistěte, jak [udělit místně spravované partnerské účty přístup k cloudovým prostředkům pomocí spolupráce Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).