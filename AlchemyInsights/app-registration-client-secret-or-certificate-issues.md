---
title: Tajný klíč klienta registrace aplikace nebo problémy s certifikátem
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
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951486"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Tajný klíč klienta registrace aplikace nebo problémy s certifikátem

Vyprší platnost tajného klíče klienta aplikace?

Bez ohledu na to, jak byla registrovaná aplikace vytvořena, ať už prostřednictvím standardního registračního procesu na portálu pro registraci aplikací nebo v případě, že hlavní povinný objekt služby byl vytvořen ve vašem tenantovi pomocí souhlasu aplikace, bude potřeba vytvořit nový tajný klíč klienta před vypršením platnosti aktuálního klienta a aktualizovat ho v souvisejícím kódu aplikace. Maximální doba platnosti je 2 roky. Jako připomenutí musí být tajná hodnota zaznamenaná, protože už nebude viditelná po opuštění stránky registrace aplikací na portálu. Další informace najdete v tématu [Rychlý start: Registrace aplikace](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) v Microsoft identity platform a Doporučené postupy pro [Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

Další informace najdete v [tématu Vytvoření aplikace Azure AD & instančního](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)objektu na portálu – Microsoft identity platform .
