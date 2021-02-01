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
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063592"
---
# <a name="configure-and-customize-applications"></a>Konfigurace a přizpůsobení aplikací

**Konfigurace aplikací**

1. Rychlý start: Konfigurace vlastností aplikace ve vašem [tenantovi Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) ukazuje, jak nakonfigurovat některé vlastnosti aplikace.
2. Pro integraci vašich aplikací se službou [](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) Azure Active Directory jsme vyvinuli kolekci kurzů, které vás pomůžou projít konfigurací.
3. [Návod na konfiguraci aplikace Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) aplikace pomáhá pochopit, jak nakonfigurovat aplikaci proxy aplikace v Azure AD k vystavení místních aplikací do cloudu.
4. [Stažení příkazu PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)a konfigurace aplikace: Postupujte podle pokynů v článku Konfigurace *příkazu PingAccess* pro Azure AD k ochraně aplikací publikovaných pomocí proxy aplikace Microsoft Azure AD na webu Ping Identity a stáhněte si nejnovější verzi příkazu PingAccess.

**Chyby nesprávně nakonfigurovaných aplikací (AADSTS650056)**

1. Ujistěte se, že k aplikaci přistupujete z přihlašovací adresy, kterou vám poskytl vlastník aplikace. V opačném případě se přihlaste do aplikace běžným procesem. Ve většině případů to bude automaticky vyřešit přirozeně. Pokud ne, pomůže vám tento příspěvek odstranit a vyřešit ho.
2. **Pokud vaše organizace aplikaci vlastní** (to znamená, že registrace aplikace je ve vaší organizaci):
    - Doporučujeme minimálně přidat nebo delegovat `User.Read` `openid` oprávnění z Microsoft **Graphu.**
    - Zajistěte, aby aplikace a všechna její oprávnění byly souhlasné. Můžete to ověřit tak, že se podíváme na sloupec **Stav** registrace aplikace v rámci **oprávnění API.**
    - V některých případech může být aplikace třetí strana, ale může být zaregistrovaná ve vaší organizaci. Potvrďte, jestli je tato aplikace uvedená ve vašich registracích aplikací (ne v aplikacích Enterprise).
    - Pokud se bude tato chybová zpráva dále zobrazit. Pak budete možná muset vytvořit adresu URL souhlasu popsanou v **kroku 4.**
3. **Pokud vaše organizace není vlastníkem aplikace a** používá ji jako aplikaci jiného výrobce:
    - Pokud jste globální správce nebo správce společnosti, měla by se zobrazit obrazovka pro udělení souhlasu. Ujistěte se, že **zaškrtáte políčko "Souhlas jménem vaší organizace".**
    - Pokud se obrazovka pro udělení souhlasu nez zobrazí, odstraňte aplikaci Enterprise a zkuste to znovu.
    - Pokud se vám bude tato chybová zpráva dále zobrazit. Pak budete možná muset vytvořit adresu URL souhlasu popsanou v **kroku 4.**
4. **Ruční vytvoření** adresy URL souhlasu, která se má použít: Pokud je aplikace určená pro přístup k určitému prostředku, možná nebudete moct použít tlačítka souhlasu z portálu Azure Portal, budete muset ručně vygenerovat adresu URL svého souhlasu a použít tuto adresu.
    - Musíte získat informace od vlastníka `{App-Id}` `{App-Uri-Id}` aplikace. `{Tenant-Id}` bude identifikátorem vašeho tenanta. Bude to buď vaše `yourdomain.onmicrosoft.com` ID adresáře, nebo vaše.
    - Pokud se aplikace k prostředku přistupuje sám, bude stejná `{App-Id}` `{App-Uri-Id}` a bude stejná.
5. Další informace najdete v tématu Problémy s přihlašováním k nakonfigurovaným aplikacím založeným na jednotném [přihlašování na základě SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Přizpůsobení aplikací**

- Přidání značky na přihlašovací stránku Azure Active Directory vaší organizace – k zajištění konzistentního vzhledu přihlašovacích stránek Azure Active Directory [(Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) AD) použijte logo vaší organizace a vlastní barevná schémata.
- [Přidejte vlastní název domény pomocí portálu Azure Active Directory –](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) každý nový tenant Azure AD má počáteční název domény. Původní název domény nemůžete změnit ani odstranit, ale můžete přidat názvy vaší organizace. Přidáním vlastních názvů domén můžete vytvářet dobře známá uživatelská jména.
