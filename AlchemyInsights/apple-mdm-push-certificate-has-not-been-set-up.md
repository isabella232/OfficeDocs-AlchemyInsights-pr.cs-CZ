---
title: Certifikát Apple MDM Push certificate nebyl nastaven.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438852"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Certifikát Apple MDM Push certificate nebyl nastaven.

Pro vaše předplatné nebyl nakonfigurován certifikát Apple MDM (označovaný také jako certifikát Služby nabízených oznámení Apple (APNS). Bez nakonfigurovaného nabízeného certifikátu Apple MDM nemůžete zaregistrovat a spravovat zařízení se systémem iOS a Mac OS. Po přidání certifikátu do Intune si uživatelé můžou nainstalovat aplikaci Portál společnosti a zaregistrovat svá iOS zařízení.

1. Vyberte **možnost Souhlasím.** a udělí společnosti Microsoft oprávnění k odesílání dat společnosti Apple.

2. Vyberte **Stáhnout csr** žádost o podepisování certifikátu Intune, která je vyžadována k vytvoření nabízeného certifikátu Apple MDM. Soubor se používá k vyžádání certifikátu vztahu důvěryhodnosti z portálu Apple Push Certificates Portal.

3. Výběrem **možnosti Vytvořit nabízený certifikát MDM přejděte** na portál Apple Push Certificates Portal. Přihlaste se pomocí firemního Apple ID a pak vyberte **Vytvořit certifikát**. Vyberte **Vybrat soubor**, vyhledejte soubor žádosti o podpis certifikátu a pak zvolte **Nahrát**. Na stránce Potvrzení zvolte **Stáhnout, chcete-li** stáhnout soubor certifikátu (.pem) a uložit soubor místně.
 
**Poznámka:** Certifikát je spojený s Apple ID použitým k jeho vytvoření. Osvědčeným postupem je použití firemního Apple ID pro úkoly správy a ujistěte se, že poštovní schránka je monitorována více než jednou osobou nebo pomocí distribučního seznamu. Nikdy nepoužívejte osobní Apple ID. K obnovení apple push certifikátu každých 12 měsíců použijte stejné Apple ID.
 
4. Zadejte Apple ID použité k vytvoření nabízeného certifikátu Apple MDM. Toto ID zaznamenejte jako připomenutí, kdy potřebujete certifikát obnovit.

5. Přejděte do souboru certifikátu (.pem), zvolte **Otevřít**a pak zvolte **Nahrát**. S nabízeným certifikátem může Intune zaregistrovat a spravovat zařízení Apple.