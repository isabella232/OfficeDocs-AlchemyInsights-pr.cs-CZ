---
title: Vyhledání chybějících aplikací v okně Registrace aplikací
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057095"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Vyhledání chybějících aplikací v okně Registrace aplikací

1. Aplikace na portálu pro registraci aplikací se nejdou najít.

    Pokud je aplikace aplikace s více tenanty a zaregistrovaná v jiném tenantovi, nezobrazí se v okně Registrace aplikace. Může se ale zobrazit v okně Enterprise aplikace, jakmile se k němu dostanete (po souhlasu) a ve vašem tenantovi se vytvoří hlavní objekt služby. Další informace najdete v tématu [Aplikace & instanční objekty v Azure AD – Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. Aplikace se nedaří zobrazit v okně Registrace aplikací, i když jste správce.

    Ujistěte se prosím, že jste ve správném adresáři na portálu Azure Portal.
3. Moje aplikace není uvedená v Enterprise Aplikace, ale zobrazí se při dotazu na příkaz PowerShellu.

    Někdy se aplikace po odstranění z portálu Azure Portal na portálu nezminí, ale možná nebyla úplně odstraněna. Další informace najdete tady:
    - Seznam dříve odstraněných aplikací můžete načíst a zjistit, jestli se aplikace v seznamu zobrazuje pomocí příkazu PowerShellu: **Get-AzureADDeletedApplication**. Další informace najdete v tématu [Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - Pokud chcete aplikaci úplně odebrat, můžete v PowerShellu vyzkoušet toto: **Remove-AzureADApplication -ObjectId**. Další informace najdete v tématu [Odebrání AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Můžete také zkusit obnovit odstraněnou aplikaci pomocí následujícího příkazu PowerShellu: **Obnovit AzureADDeletedApplication -ObjectId**. Další informace najdete v tématu [Obnovení AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Nemůžu najít seznam všech předinstalovaných podnikových aplikací v novém tenantovi Azure.

    Ve výchozím nastavení nejsou v Azure AD žádné předinstalované podnikové aplikace. Musíte ho přidat ručně z možnosti Nová aplikace tak, že ji budete procházet z galerie Azure AD nebo přidáte aplikaci, která není galerie. Další informace najdete v tématu Rychlý start: Přidání aplikace do tenanta [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Pokud jste globální správce, můžete se ke svým aplikacím snadno dostat pomocí [Microsoft 365 spouštěče aplikací.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Moje aplikace se nedaří najít na portálu Moje aplikace.

    Ujistěte se, že aplikace nejsou na stránce kolekce Moje aplikace skryté. Další informace najdete v tématu [Kolekce (preview) na portálu Moje aplikace – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Pokud chcete spustit aplikace z portálu Moje aplikace, podívejte se na & používání aplikací na portálu Moje aplikace [– Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Office 365 Aplikace Mover se po instalaci nezobrazuje v okně Enterprise aplikace.

    Aplikace Office 365 Mover je multitenantní aplikace, která se nemusí přidávat do služby AAD pomocí oddílu Galerie aplikací v části Enterprise registrace aplikací. Pokud chcete Office 365 aplikace Mover, jednoduše se přihlaste k aplikaci a požádá o souhlas uživatele s oprávněními. Jakmile uživatel souhlas poskytne, tato aplikace se automaticky přidá do tenanta s ID e-mailu, ke které jste se přihlásili.

    Po přihlášení k aplikaci byste měli být schopni najít položku této aplikace v okně Enterprise aplikace v AAD. Aplikaci musíte vyhledat tak, že zadáte celé jméno, tj. "Office 365 Mover" nebo jednoduše vyhledáte "office" a aplikace by měla být v seznamu. Další informace najdete v článku Office 365 Mover říká, že už je nainstalovaný, ale není uvedený v [galerii Enterprise aplikací](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html).
8. Rychlý start: Zobrazení seznamu aplikací, které používají vašeho [tenanta Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) pro správu identit, ukazuje, jak zobrazit aplikace , které jsou už nastavené tak, aby jako svého poskytovatele identity (IdP) používejte tenanta Azure AD.
9. [Řešení běžných problémů s přidáním nebo odebráním](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) aplikace do Azure Active Directory pomáhá pochopit běžné problémy, se které lidé při prohlížení aplikací v Azure Active Directory.
