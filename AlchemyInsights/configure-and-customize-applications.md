---
title: Konfigurace a přizpůsobení aplikací
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
- "9004334"
- "7733"
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044981"
---
# <a name="configure-and-customize-applications"></a>Konfigurace a přizpůsobení aplikací

**Konfigurace aplikací**

1. [Rychlý start: Konfigurace vlastností aplikace v tenantovi Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) ukazuje, jak nakonfigurovat některé z vlastností aplikace.
2. Pro integraci aplikací s Azure Active Directory jsme vyvinuli kolekci kurzů, které vás provede konfigurací. [](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)
3. [Jak nakonfigurovat aplikaci Proxy aplikací](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) vám pomůže pochopit, jak nakonfigurovat aplikaci Proxy aplikací v Azure AD tak, aby vystavěly vaše místní aplikace do cloudu.
4. [Stáhněte si PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)Microsoft Azure AD nakonfigurujte aplikaci : Postupujte podle pokynů v tématu Konfigurace *pingaccessu* pro Azure AD k ochraně aplikací publikovaných pomocí proxy serveru aplikace Microsoft Azure AD na webu Ping Identity a stáhněte si nejnovější verzi pingaccessu.

**Chybně nakonfigurovaná aplikace (AADSTS650056)**

1. Ujistěte se, že k aplikaci přistupujete z přihlašovací adresy poskytnuté vlastníkem aplikace. V opačném případě se přihlaste k aplikaci běžným procesem. Ve většině případů se to automaticky vyřeší přirozeně. Pokud ne, pomůže vám tento příspěvek vyřešit a vyřešit problém.
2. **Pokud vaše organizace vlastní aplikaci** (což znamená, že registrace aplikace je ve vaší organizaci):
    - Minimálně doporučujeme přidat nebo delegovat oprávnění od `User.Read` `openid` **Graph** Microsoftu.
    - Ujistěte se, že aplikace a všechna její oprávnění jsou s tím souhlasné. Můžete to ověřit tak, že se podíváme na sloupec **Stav** registrace aplikace v rámci oprávnění **rozhraní API**.
    - V některých situacích může být aplikace třetí stranou, ale může být zaregistrovaná ve vaší organizaci. Potvrďte, jestli je tato aplikace uvedená ve vašich registracích aplikací (Enterprise aplikací).
    - Pokud se vám tato chybová zpráva dál zobrazí. Pak budete možná muset vytvořit adresu URL souhlasu popsanou v **kroku 4**.
3. **Pokud vaše organizace není vlastníkem aplikace a** používá ji jako aplikaci třetí strany:
    - Pokud jste správcem global/company, měla by se zobrazit obrazovka souhlasu. Ujistěte se, že zaškrtáte **políčko "Souhlas jménem vaší organizace"**.
    - Pokud se obrazovka souhlasu nevidí, odstraňte aplikaci Enterprise a zkuste to znovu.
    - Pokud se vám tato chybová zpráva dál zobrazí. Pak budete možná muset vytvořit adresu URL souhlasu popsanou v **kroku 4**.
4. **Ručně vytvořte** adresu URL souhlasu, která se má použít: Pokud je aplikace navržená pro přístup k určitému prostředku, možná nebudete moct použít tlačítka Souhlas z portálu Azure Portal, budete muset ručně vygenerovat adresu URL vlastního souhlasu a použít tuto adresu.
    - Budete muset získat a od `{App-Id}` `{App-Uri-Id}` vlastníka aplikace. `{Tenant-Id}` bude identifikátor vašeho tenanta. Bude to buď vaše `yourdomain.onmicrosoft.com` ID adresáře, nebo vaše ID adresáře.
    - Pokud aplikace k prostředku přistupuje sama, bude mít stejný `{App-Id}` `{App-Uri-Id}` název a.
5. Další informace najdete v tématu Problémy s přihlášením k aplikacím nakonfigurovaným pomocí jednotného přihlašování [založeného na protokolu SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**Přizpůsobení aplikací**

- [Přidání značky](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) na přihlašovací stránku vaší organizace – pomocí loga vaší organizace Azure Active Directory vlastních barevných schémat zajistíte konzistentní vzhled přihlašovacích stránek Azure Active Directory (Azure AD).
- [Přidejte svůj vlastní název domény](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) pomocí Azure Active Directory – Každý nový tenant Azure AD má počáteční název domény. Počáteční název domény nemůžete změnit ani odstranit, ale můžete přidat názvy vaší organizace. Přidáním vlastních názvů domén můžete vytvářet uživatelská jména, která znají vaši uživatelé.
