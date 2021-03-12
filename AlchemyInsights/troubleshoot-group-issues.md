---
title: Poradce při potížích se skupinou
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "50713439"
---
# <a name="troubleshoot-group-issues"></a>Poradce při potížích se skupinou

**Potřebuji přiřadit skupinu k roli Azure AD**

Pokud chcete přiřadit skupinu Azure Active Directory (AD) k roli Azure AD, postupujte takto:

1. Vytvoření nové skupiny – vytvoření nové skupiny:

    a. Přihlaste se do Centra pro správu Azure AD pomocí privilegovaného správce rolí nebo oprávnění globálního správce. 
    b. V seznamu Skupiny služby Azure Active Directory > skupiny > Skupiny a > novou skupinu. 
    c. Vytvořte skupinu.

2. Přiřaďte skupině roli buď během vytváření skupiny, nebo i po vytvoření skupiny.

    a. Pokud chcete přidělit skupině roli v okamžiku vytvoření skupiny, můžete této skupině přiřadit roli pomocí přepínače Azure AD a vytvořit skupinu.
    b. Pokud chcete po vytvoření přiřadit skupině roli, přejděte na kartu Přiřazené role pro nově vytvořenou skupinu a přiřaďte ji skupině.

**Potřebuji spravovat členství ve skupině, která je přiřazená k roli Azure AD**

1. Aby se předešlo převýšení oprávnění, může ve výchozím nastavení měnit členství ve skupině, která je přiřazená k roli, jenom privilegovaný správce role a globální správce. Mohou se však rozhodnout přiřadit vlastníka takové skupiny a delegovat tento úkol. Další informace najdete v tématu [Použití cloudových skupin ke správě přiřazení rolí v Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)
2. Časté otázky a tipy pro odstraňování potíží při přiřazování rolí skupinám v Azure AD najdete v tématu Řešení potíží s [rolemi přiřazenými ke cloudovým skupinám.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)

**Dynamické skupiny**

1. Pokud nemůžete najít předdefinové atributy uživatele, ujistěte se, že je tento atribut v seznamu podporovaných vlastností.
2. Pokud hledáte předdefinové atributy zařízení, ujistěte se, že atribut je v seznamu atributů zařízení. 
3. Kromě předdefinových atributů uživatele a zařízení můžete také použít [atributy rozšíření.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) Po synchronizaci atributů rozšíření z místní ad Windows Serveru nebo z připojené aplikace SaaS by se atributy měly zobrazit v rozevíracím seznamu Tvůrce pravidel. Název vlastního atributu se v adresáři nachází dotazem na atribut uživatele pomocí PowerShellu a vyhledáním názvu atributu. Lze je také použít při vytváření pravidel v syntaxi pravidla.
4. Ujistěte se, že váš tenant má odpovídající licenci. Dynamické skupiny vyžadují, aby měl tenant licenci Azure AD P1 Premium. Seznam plánů licence Azure AD najdete [tady.](https://azure.microsoft.com/pricing/details/active-directory/) Licenční plány Enterprise Mobility + Security najdete [tady.](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. Ověřte, že je role uživatele, který dynamickou skupinu vytváří, globálním správcem, správcem Intune, správcem skupiny nebo správcem uživatele.
6. Povolte prosím čas, aby se skupina mohla naplnit. V závislosti na velikosti vašeho tenanta může trvat až 24 hodin, než se skupina načtou nebo po změně pravidla.
7. Další informace najdete v článku [Vytvoření pravidel založených na atributech pro dynamické členství ve skupinách.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)

**Potřebuji odstranit skupinu**

1. Skupiny se odstraňovat z adresáře pomocí rutiny Remove-AzureADGroup Azure AD Powershellu.
2. Než se pokusíte odstranit synchronizované skupiny v Azure AD, ujistěte se, že jste odstranili všechny přiřazené licence, abyste se vyhnuli chybám.
3. Další informace o odstraňování skupin najdete v tématu [Odstranění skupiny s přiřazenou licencí.](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)

**Potřebuju obnovit odstraněnou skupinu**

1. Když odstraníte skupinu Office 365, můžete ji obnovit až 30 dní před trvalým odstraněním. Po trvalém odstranění už nebude možné skupinu obnovit. Další informace o obnovování [skupin najdete tady.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)
2. Tato funkce není podporovaná u skupin zabezpečení a distribučních skupin.
3. Ujistěte se, že máte oprávnění k obnovení skupiny Office 365. Můžou ji obnovit globální správci, správci skupin, správci uživatelských účtů, správci služeb Intune, partneři na úrovni 1 nebo úroveň2 a vlastník skupiny.
4. Když se dynamická skupina odstraní a obnoví, bude vidět jako nová skupina a znovu se vyplní podle pravidla. Tento proces může trvat až 24 hodin.
5. Další informace o obnovení odstraněné skupiny najdete v článku Obnovení odstraněné skupiny [Office 365](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)v Azure Active Directory.

**Konfigurace zásad vypršení platnosti skupiny**

1. Tato funkce je podporovaná jenom pro skupiny Office 365, ne pro skupiny zabezpečení a distribuční skupiny.
2. Konfigurace a používání zásad vypršení platnosti pro skupiny Office 365 vyžaduje licenci Azure AD Premium.
3. Pro skupiny Office 365 v tenantovi se v současné době může nakonfigurovat jenom jedna zásada vypršení platnosti.
4. Skupinu můžou obnovit jenom globální správci, správci skupin, správci uživatelů a vlastník skupiny.
5. Pokud vypršela platnost skupiny Office 365, odstraní se a bude možné ji obnovit až do 30 dnů před trvalým odstraněním. Po trvalém odstranění už nebude možné skupinu obnovit. Další informace o obnovování [skupin najdete tady.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Automatické prodlužování na základě aktivit**

Aktivity uživatelů ze SharePointu, Outlooku a Teams mohou aktivovat automatické prodlužování platnosti skupiny. Aktivity se kontroluly 35 dnů před vypršením platnosti skupiny. Pokud dojde během životního cyklu aktuální skupiny k aktivitě, skupina se automaticky obnoví a vlastníkům skupiny se nepošla e-mailová oznámení.

**Časování oznámení pro skupiny s vypršenou platností**

1. E-mailová oznámení se posílají vlastníkům skupiny Office 365 30 dní, 15 dní a 1 den před vypršením platnosti skupiny.
2. Při prvním nastavení vypršení platnosti se všechny skupiny, které jsou starší než interval vypršení platnosti, nastaví 35 dní do vypršení platnosti.
3. Datum vypršení platnosti skupiny se vypočítá na základě data prodloužení platnosti skupiny, nikoli na základě data aktualizace zásad. Pokud se zásady vypršení platnosti aktualizují, datum vypršení platnosti se nezmění.
4. Další informace najdete v článku Zásady vypršení platnosti skupiny a [e-maily](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) o obnovení a Obnovení odstraněné skupiny [Office 365](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)v Azure Active Directory.

**Oprávnění k vytvoření skupiny**

Ujistěte se, že máte oprávnění k vytvoření nové skupiny. Globální správci můžou vytváření skupin na portálu Azure nebo na přístupových panelech zakázat. K vytvoření nové skupiny nebo k tomu, abyste získali příslušná oprávnění, budete možná potřebovat správce.

1. [Vytvoření nové skupiny a přidání členů na portálu Azure Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Vytváření skupin v PowerShellu MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Zakázání vytváření skupin v PowerShellu](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Správa uživatelů, kteří mohou vytvářet skupiny v Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Zakázání uvítacího oznámení Office 365 přes PowerShell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Role pro správu Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Správa oprávnění pro vytváření skupin**

1. Globální správci můžou spravovat oprávnění k vytváření skupin pro zabezpečení nebo skupiny Office 365 vytvořené na portálu Azure nebo na panelu Pro přístup nastavením Uživatelé můžou vytvářet skupiny zabezpečení na portálech **Azure nebo** uživatelé můžou vytvářet skupiny **Office 365** v nastavení portálů Azure v části Všechny skupiny > Obecné **(Nastavení).**
2. Pokud máte licenci Azure AD P1 Premium, můžete vytváření skupin omezit na výběr skupiny uživatelů.

**Zakázání úvodního oznámení pro nové členy skupiny Office 365**

Uvítací oznámení odeslané uživatelům přidaných do skupin Office 365 můžete v PowerShellu zakázat nastavením na `UnifiedGroupWelcomeMessageEnabled` False (Nepravda).  Informace o tomto nastavení najdete [tady.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)













