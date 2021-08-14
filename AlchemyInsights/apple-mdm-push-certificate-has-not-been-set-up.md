---
title: Nabízený certifikát Apple MDM není nastavený.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 4f8e3502a7be35b5579ec1436852fe2bff9b1316891c7a9020f6f5f4767b3d88
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931521"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Nabízený certifikát Apple MDM není nastavený.

Nabízený certifikát Apple MDM (označovaný taky jako certifikát APNS (Apple Push Notification Service) není pro vaše předplatné nakonfigurovaný. Bez nakonfigurovaného nabízeného certifikátu Apple MDM nemůžete zaregistrovat a spravovat zařízení s iOS a Mac OS. Po přidání certifikátu do Intune si uživatelé instalují aplikaci Portál společnosti pro registraci zařízení s iOSem.

1. Vyberte **"Souhlasím".** společnosti Microsoft udělit oprávnění k odesílání dat společnosti Apple.

2. Pokud chcete vytvořit nabízený certifikát Apple MDM, vyberte Stáhnout **cs-CZ** žádost o podpis certifikátu Intune. Soubor se používá k vyžádání certifikátu vztahu důvěryhodnosti z portálu Apple Push Certificates Portal.

3. Vyberte **Vytvořit nabízený certifikát MDM a** přejděte na portál Apple Push Certificates Portal. Přihlaste se svým firemním Apple ID a pak vyberte **Vytvořit certifikát**. Vyberte **Zvolit soubor,** přejděte na soubor žádosti o podpis certifikátu a pak zvolte **Upload**. Na stránce Potvrzení zvolte **Stáhnout** a stáhněte si soubor certifikátu (.pem) a soubor uložte místně.
 
**Poznámka:** Certifikát je přidružený k Apple ID použitému k jeho vytvoření. Jako osvědčený postup použijte firemní Apple ID pro úkoly správy a ujistěte se, že poštovní schránku sleduje víc než jedna osoba nebo pomocí distribučního seznamu. Nikdy nepoužívejte osobní Apple ID. K prodloužení apple push certifikátu každých 12 měsíců použijte stejné Apple ID.
 
4. Zadejte Apple ID použité k vytvoření nabízeného certifikátu Apple MDM. Nahrajte toto ID jako připomenutí, kdy potřebujete certifikát prodloužit.

5. Přejděte do souboru certifikátu (.pem), zvolte **Otevřít** a pak zvolte **Upload**. Pomocí nabízeného certifikátu může Intune zaregistrovat a spravovat zařízení Apple.