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
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404295"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="f5b7e-102">Tajný klíč klienta registrace aplikace nebo problémy s certifikátem</span><span class="sxs-lookup"><span data-stu-id="f5b7e-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="f5b7e-103">Vyprší platnost tajného klíče klienta aplikace?</span><span class="sxs-lookup"><span data-stu-id="f5b7e-103">Application client secret expiring?</span></span>

<span data-ttu-id="f5b7e-104">Bez ohledu na to, jak byla registrovaná aplikace vytvořena, ať už prostřednictvím standardního registračního procesu na portálu pro registraci aplikací nebo v případě, že hlavní povinný objekt služby byl vytvořen ve vašem tenantovi pomocí souhlasu aplikace, bude potřeba vytvořit nový tajný klíč klienta před vypršením platnosti aktuálního klienta a aktualizovat ho v souvisejícím kódu aplikace.</span><span class="sxs-lookup"><span data-stu-id="f5b7e-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="f5b7e-105">Maximální doba platnosti je 2 roky.</span><span class="sxs-lookup"><span data-stu-id="f5b7e-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="f5b7e-106">Jako připomenutí musí být tajná hodnota zaznamenaná, protože už nebude viditelná po opuštění stránky registrace aplikací na portálu.</span><span class="sxs-lookup"><span data-stu-id="f5b7e-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="f5b7e-107">Další informace najdete v tématu Rychlý start: Registrace aplikace na platformě [identit Microsoftu a](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) Osvědčené postupy pro platformu identit [Microsoftu](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span><span class="sxs-lookup"><span data-stu-id="f5b7e-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="f5b7e-108">Další informace najdete v [tématu Vytvoření aplikace Azure AD & instančního](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)objektu na portálu – platforma identit Microsoftu .</span><span class="sxs-lookup"><span data-stu-id="f5b7e-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
