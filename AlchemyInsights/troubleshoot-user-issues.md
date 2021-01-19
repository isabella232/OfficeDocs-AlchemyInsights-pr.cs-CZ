---
title: Poradce při potížích s uživatelem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900805"
---
# <a name="announcements"></a>Hlášení

Postupujte podle pokynů Google na testovací kompatibilitu a otestujte, jestli jsou vaše aplikace ovlivněné. Příručka k webu Google je k dispozici v https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Při přihlašování uživatelů pomocí účtů Google pro příjemce se ujistěte, že používáte systémové webzobrazení nebo systémový prohlížeč. Další informace najdete v článku [problémy s přihlášením k aplikacím pomocí prohlížeče Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**V adresáři Azure AD nemůžu vytvořit nového uživatele**

Pokud chcete vyřešit problém s tím, že se vám nedaří vytvořit nového uživatele v Azure AD, udělejte toto:

1. Zkontrolujte, jestli máte oprávnění vytvořit nového uživatele. Pouze role Globální správce nebo Správce uživatelů v Azure Active Directory (AD) může vytvořit nového standardního uživatele. Pokud nejste v některé z těchto rolí, požádejte správce, aby vás přidal do jedné z těchto rolí, nebo vytvořte nový uživatelský účet.
2. Zkontrolujte, jestli je uživatelské jméno v doméně, která je ověřená v Azure AD. Pokud v Azure AD nemáte nějaké ověřené vlastní názvy domén, můžete použít počáteční doménu Azure AD, která končí na *. onmicrosoft.com.
3. Ujistěte se, že uživatelské jméno je v doméně, která není federované pro Azure AD z vaší místní služby AD. Uživatele nelze do cloudu přidat s názvy domén, které jsou federované z místního.
4. Ujistěte se, že už žádný jiný uživatel ani kontakt nemá uživatelské jméno, které chcete novému uživateli přiřadit. Uživatelská jména musí být v Azure AD jedinečná.
5. Viz [role a správci Azure AD](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pro Azure AD.
6. Podívejte se na [názvy domén](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) pro Azure AD.
7. Podívejte se na [protokoly auditování](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) , kde najdete podrobnější informace o nedávno vytvořeném nebo odstraněném uživateli, jako je osoba provedená akce a kdy.
8. Další informace o přidávání nových uživatelů najdete v článku [Vytvoření nového uživatele v Azure AD pomocí portálu Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Další informace o oprávněních rolí správce v Azure AD najdete v tématu [role pro správu Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Podrobnosti o vytvoření uživatele pomocí Azure AD PowerShellu najdete v tématu [Azure AD PowerShell pro vytvoření nového uživatele](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problém s samoobslužným registrem**

Pokud chcete řešit problémy týkající se registrace pro samoobslužné služby, postupujte takto:

1. Abyste mohli používat samoobslužné zápisy s aplikacemi, nejdřív povolte pro tenanta registraci samoobslužné služby. 
2. Pokud chcete povolit aplikaci pro podporu samoobslužné registrace, přidejte ji do svého uživatelského toku. Při příštím přechodu na přihlašovací stránku této aplikace se zobrazí možnost **_žádný účet? Vytvořte si ho!_* _. Tím se spustí samoobslužný proces přihlašování.
3. Informace o tom, jak používat samoobslužné přihlašovací údaje k naplnění organizace v Azure AD, najdete v tématu [samoobslužné registrace pro Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Po přidružení toku uživatelů k jedné nebo více aplikacím se uživatelé, kteří tuto aplikaci navštíví, budou moct zaregistrovat a získat účet hosta pomocí možností konfigurovaných v toku uživatelů. Další informace o tom, jak si zaregistrovat a získat účet hosta, mohou zobrazit [samoobslužné registrace pro uživatele typu Host](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Problém s pozváním externího uživatele**

Pokud chcete řešit problémy s pozváním externích uživatelů, postupujte takto:

Ujistěte se, že pozvánku uživatele posíláte na e-mailovou adresu odpovídající jménu, pod kterým se uživatel přihlašuje. Pokud odešlete pozvánku na e-mailovou adresu proxy uživatele, uživatel ji nemůže uplatnit. Další informace najdete v tématu [dokumentace k Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Nelze přiřadit licence uživateli**

Pokud chcete řešit problémy s přidělováním licencí uživatelům, postupujte takto:

1. Pokud chcete spravovat uživatelské licence, ujistěte se, že používáte účet s jednou z povinných rolí správců: globální správce, správce licencí nebo Správce uživatelů. Roli uživatele můžete zkontrolovat na kartě **role adresáře** v okně uživatel.
2. Pokud používáte Azure Portal a nedaří se zadání licence, klikněte na oznámení v pravém horním rohu. Otevře se okno s podrobnostmi o chybě. Ve většině případů, kde je váš problém dostatečně srozumitelný.
3. Před přidělením licence uživateli se ujistěte, že je pro daného uživatele nastavená vlastnost **umístění používání** . Ověřte, jestli uživatel tuto vlastnost nastavil, a to tak, že si na kartě profilu zobrazí kartu **profil** .
4. Ujistěte se, že je k dispozici dostatek licencí pro produkt, který chcete přiřadit. Počet dostupných licencí na portálu Azure se zobrazuje v [Azure Active Directory – licence pro > – > všechny produkty](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Je možné, že uživatel už má jinou licenci, jejíž služby jsou v konfliktu s podmínkami v nové licenci, kterou chcete přiřadit. Pokud má například uživatel povolenou službu Exchange Online (plán 1), nebudete moct přiřadit licenci k Exchangi Online (plán 2). Pokud chcete povolit nové přiřazení licence, zakažte některou ze služeb. Pokud používáte Azure Portal nebo rutiny PowerShellu, Stránka s **podrobnostmi o problému** zobrazuje seznam konkrétních služeb, které způsobují konflikt.
6. Pokud se pokoušíte odebrat licenci a nedaří se vám to, že uživatel bude mít k dispozici jiné licence, které jsou závislé na službách, které chcete odebrat. Pokud používáte Azure Portal nebo rutiny PowerShellu, zobrazí se chybová zpráva o konkrétních službách, které mají závislosti.
7. Pokud chcete zjistit, proč byla licence přidána nebo odebrána od uživatele (například kdo jiný ve vaší organizaci mohl provést změny), zkontrolujte protokoly auditování. Nastavením filtru na **aktivity licencí** zobrazíte všechny změny, včetně "herce", který je provedl.
8. Pokud používáte Exchange Online, můžou se některé uživatele ve vašem tenantovi nesprávně konfigurovat se stejnou hodnotou adresy proxy. V takových případech se může stát, že při selhání licence se zobrazí obecné chybové zprávy. [Tento článek](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) obsahuje další informace o tomto problému, včetně informací o [tom, jak se připojit k Exchangi Online pomocí vzdáleného PowerShellu](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Pokud chcete zjistit, kteří uživatelé ve vašem tenantovi mají stejnou adresu proxy, spusťte tuto rutinu Exchange Online:

Funguje

Get-Recipient | kde {$ _. EmailAddresses-Match <user principal name> } | fL Name, RecipientType, EmailAddresses





