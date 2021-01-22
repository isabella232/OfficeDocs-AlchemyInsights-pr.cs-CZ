---
title: Bezproblémové problémy s přihlášením uživatele k jednotnému přihlašování
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935092"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Bezproblémové problémy s přihlášením uživatele k jednotnému přihlašování

Po ověření uživatele prohlížeč uloží přihlašovací údaje uživatele do mezipaměti, aby se aplikace ve stejném prohlížeči automaticky přihlašoval pomocí stejného účtu. Může to ztížit jinému nebo jednomu uživateli přihlášení k více účtům na jednom zařízení. Řešení: 1. Zkuste se přihlásit v jiném prohlížeči. 2. Vymažte mezipaměť a soubory cookie prohlížeče a zkuste se znovu přihlásit.

Pokud máte pořád potíže s přihlášením, doporučujeme tento postup diagnostikovat a zautomatizování:

1. Nainstalujte si rozšíření my [Apps Secure Browser Extension](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) (Rozšíření zabezpečených prohlížečů), které pomáhá Azure Active Directory (Azure AD) poskytovat lepší diagnostiku a řešení při používání testovacích prostředí na portálu Azure Portal.
2. Reprodukovat chybu pomocí testování prostředí na stránce pro konfiguraci aplikace na portálu Azure Portal. Další informace najdete v tématu Ladění aplikací pro jednotné přihlašování založené na systému [SAML.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Pokud používáte testování na portálu Azure Portal s rozšířením My Apps Secure Browser Extension (Rozšíření zabezpečeného prohlížeče Moje aplikace), můžete **krok 4 přeskočit.**
4. Otevření stránky konfigurace jednotného přihlašování založené na serveru SAML:
    - Otevřete [portál Azure Portal](https://portal.azure.com/) a přihlaste se jako **globální správce** nebo **správce.**
    - Otevřete rozšíření **Azure Active Directory tak,** že **v** horní části hlavní navigační nabídky na levé straně vyberete Všechny služby.
    - Do vyhledávacího pole filtru zadejte Azure Active Directory a vyberte **položku Azure Active Directory.**
    - V **levé navigační nabídce** Azure Active Directory vyberte Podnikové aplikace.
    - Výběrem **možnosti Všechny** aplikace zobrazte seznam všech vašich aplikací. Pokud tu aplikaci, kterou chcete zobrazit, nevidíte, použijte ovládací  prvek Filtr v  horní části seznamu Všechny aplikace a nastavte možnost Zobrazit na **Všechny aplikace.** 
    - Vyberte aplikaci, kterou chcete nakonfigurovat pro jednotné přihlašování.
    - Po načtení aplikace **vyberte** z levé navigační nabídky aplikace jednotné přihlašování.
    - Vyberte **jednotné přihlašování založené na systému SAML.**
5. Na základě této chyby se dozvíte víc o doporučených krocích, které je vhodné provést, v tématu Problémy s přihlášením k nakonfigurovaným aplikacím založeným na jednotném přihlašování na základě [SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. Pokud chcete vyřešit jiné problémy s přihlášením uživatele, přečtěte si následující pokyny:
    - [Protokol SAML Sign-On single-Sign-On](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Postup: Řešení potíží s chybami přihlášení pomocí sestav služby Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Neočekávaná výzva k zadání souhlasu](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Chyba při souhlasu uživatele](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problémy s přihlášením z mých aplikací](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Chyba na přihlašovací stránce aplikace](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problém s přihlášením do aplikace Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
