---
title: Vytvoření uživatele
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: d86b2dd6d7915f0698cf950cd57f1065cde22219284edbbc0e64f3a5e69ff252
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896708"
---
# <a name="create-user"></a>Vytvoření uživatele

**OZNÁMENÍ:**

- [Od 4. ledna 2021 se od Googlu od 4. ledna 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) odepisování podpory pro přihlášení k WebView Otestujte, jestli vaše aplikace nemusí být ovlivněné pokyny [Společnosti Google pro](https://go.microsoft.com/fwlink/?linkid=2157323) testování kompatibility.
- Při přihlašování uživatelů pomocí spotřebitelských účtů Google se ujistěte, že používáte webové zobrazení systému nebo prohlížeč systému. Další informace najdete v tématu Problémy s přihlášením k aplikacím jenom [v prohlížeči Chrome.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Nemůžu vytvořit nového uživatele v adresáři Azure AD**

1. Ujistěte se, že máte oprávnění k vytvoření nového standardního uživatele. Nového standardního uživatele může vytvořit jenom role globálního správce nebo správce Azure Active Directory (AD). Pokud nejste v jedné z těchto rolí, požádejte správce o přidání do jedné z těchto rolí nebo o vytvoření nového uživatelského účtu.
1. Ujistěte se, že je uživatelské jméno v doméně, která je ověřená ve vaší službě Azure AD. Pokud ve službě Azure AD nemáte žádné ověřené vlastní názvy domén, můžete použít počáteční doménu Azure AD, která končí *.onmicrosoft.com.
1. Ujistěte se, že je uživatelské jméno v doméně, která není federovaná do Azure AD z místní služby AD. Uživatele nelze přidat do cloudu s názvy domén, které jsou federované z místního prostředí.
1. Ujistěte se, že žádný jiný uživatel ani kontakt už nemá uživatelské jméno, které chcete novému uživateli přiřadit. Uživatelská jména musí být jedinečná ve službě Azure AD.
1. Podívejte [se na role a správce Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pro azure AD.
1. Podívejte se [na názvy](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) domén pro azure AD.
1. Prohlédněte [si protokoly](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) auditování a podívejte se na podrobnější informace o nedávno vytvořeném nebo odstraněných uživatelech, jako je kdo akci provedl a kdy.
1. Další informace o přidávání nových uživatelů najdete v tématu Použití portálu Azure Portal k vytvoření nového [uživatele ve službě Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal).
1. [Role správy Azure AD:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)Oprávnění rolí správce v Azure Active Directory
1. K vytvoření [nového uživatele můžete taky použít Azure AD PowerShell.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
