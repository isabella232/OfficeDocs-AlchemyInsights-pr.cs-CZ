---
title: Problémy se s řízením uživatelů
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035138"
---
# <a name="user-management-issues"></a>Problémy se s řízením uživatelů

**Co se stane s aktuálními přiřazenými uživateli aplikace, když zakážem vlastnost "Přiřazení uživatele je povinné" (tato vlastnost se nastaví na Ne)?**

Zakázání **povinného přiřazení uživatele** nemá vliv na aktuálně přiřazené uživatele. Zakázání této vlastnosti umožní přístup k aplikaci jenom všem uživatelům. Všichni uvedená uživatelé a uživatelé přiřazení ke skupinám v aplikaci budou i nadále platní.

- Pokud chcete aplikaci omezit na konkrétní sadu uživatelů, podívejte se na článek – Omezení aplikace Azure AD na sadu uživatelů [– platforma identit Microsoftu | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Pokud chcete přiřazovat uživatele a skupiny, k podnikovým aplikacím v Azure Active Directory (Azure AD), ať už z webu Azure Portal, nebo pomocí PowerShellu, podívejte se na tématu Správa přiřazení uživatelů pro aplikaci v [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Pokud chcete delegovat oprávnění k vytváření a správě aplikací, podívejte se na delegování oprávnění správce správy [aplikací – Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Skrytí konkrétních podnikových aplikací** uživatelům : Pomocí následujících kroků skryjte všechny aplikace Microsoft 365 z panelu **MyApps.** Aplikace budou pořád viditelné na portálu Office 365.

 1. Přihlaste se k webu Azure Portal jako globální správce vašeho adresáře. 
 2. Vyberte **Azure Active Directory**. 
 3. Vyberte **Uživatelé**. 
 4. Vyberte **Nastavení uživatele**. 
 5. V **části Podnikové aplikace** klikněte na Spravovat způsob spouštění a prohlížení aplikací **koncovým uživatelům.** 
 6. Uživatelé **uvidí jenom aplikace Office 365 na portálu Office 365** a kliknou na **Ano.** 
 7. Klikněte na **Uložit**. 
 8. Další podrobnosti najdete v tématu skrytí podnikové aplikace z uživatelského prostředí [v Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Pokud mnoha organizacím nabízíte aplikaci Software jako služba (SaaS), můžete aplikaci nakonfigurovat tak, aby přijímaly přihlášení z libovolného tenanta Azure Active Directory (Azure AD). Tato konfigurace se nazývá "vytvoření více tenantů vaší aplikace". Uživatelé v libovolném tenantovi Azure AD se budou moct přihlásit k vaší aplikaci po souhlasu s používáním svého účtu s vaší aplikací. Další informace najdete v tématu [Vytváření aplikací, které se přihlaší k uživatelům Azure AD – platforma identit Microsoftu | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Jak může koncový uživatel získat přístup k aplikaci, jakmile je k aplikaci přiřazen?**

Každá aplikace v okně aplikace Enterprise má odkaz pro přístup koncových uživatelů. Uživatelé mají k aplikaci snadný přístup také prostřednictvím portálu **Myapps.**

- **Chcete vědět, které aplikace a typy aplikací používají uživatelé?**

Sestavy přihlášení za posledních 30 dní si můžete stáhnout z portal.azure.com > **Azure Active directory> Signins> stáhnout sestavy.**

- Zjistěte, jak udělit souhlas [správce celého tenanta](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) s aplikací a Konfigurace souhlasu [koncových uživatelů s aplikacemi](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- [Pochopte, jak souhlas funguje,](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) [a Správa souhlasu s aplikacemi](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


