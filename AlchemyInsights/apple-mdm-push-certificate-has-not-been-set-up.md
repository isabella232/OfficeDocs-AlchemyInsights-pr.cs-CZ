---
title: Nebyl nastaven nabízený certifikát Apple MDM
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
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716850"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Nebyl nastaven nabízený certifikát Apple MDM

Pro vaše předplatné není nakonfigurovaný certifikát Apple MDM pro nabízené (označované také jako certifikát APNS (Apple Push Notification Service)). Bez nakonfigurovaného účtu Apple MDM push nemůžete registrovat a spravovat zařízení s iOS a Mac OS. Po přidání certifikátu do Intune můžou uživatelé nainstalovat aplikaci Portál společnosti pro registraci zařízení s iOS.

1. Vyberte **"Souhlasím".** poskytnutí oprávnění Microsoftu k posílání dat na Apple.

2. Vyberte **Stáhnout oddělení služeb zákazníkům** : žádost o podepsání certifikátu Intune požadovaná k vytvoření certifikátu Apple MDM push. Soubor se používá k vyžádání certifikátu vztahu důvěryhodnosti na portálu Apple Push Certificates.

3. Vyberte **vytvořit certifikát MDM** pro přechod na portál Apple Push Certificates. Přihlaste se pomocí Apple ID společnosti a pak vyberte **vytvořit certifikát**. Vyberte **zvolit soubor**, přejděte do souboru žádosti o podpis certifikátu a pak zvolte **nahrát**. Na stránce s potvrzením zvolte **Stáhnout** a Stáhněte si soubor Certificate (. pem) a uložte soubor místně.
 
**Poznámka**: certifikát je přidružený k Apple ID použitému k jeho vytvoření. Nejvhodnějším postupem je použít pro úkoly správy společnost Apple ID společnosti a zkontrolovat, jestli je poštovní schránka monitorovaná více lidmi, nebo pomocí distribučního seznamu. Nikdy nepoužívejte osobní ID Apple. Pomocí stejného Apple ID prodlužte platnost certifikátu Apple Push každých 12 měsíců.
 
4. Zadejte Apple ID používané k vytvoření svého certifikátu Apple MDM push. Pokud potřebujete certifikát prodloužit, nahrajte toto ID jako připomenutí.

5. Přejděte do souboru Certificate (. pem), zvolte **otevřít**a pak zvolte **nahrát**. S certifikátem push může Intune zaregistrovat a spravovat zařízení Apple.