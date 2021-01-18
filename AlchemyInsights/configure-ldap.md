---
title: Konfigurace protokolu LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884958"
---
# <a name="configure-ldap"></a><span data-ttu-id="d49c5-102">Konfigurace protokolu LDAP</span><span class="sxs-lookup"><span data-stu-id="d49c5-102">Configure LDAP</span></span>

<span data-ttu-id="d49c5-103">Při konfiguraci protokolu LDAP postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="d49c5-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="d49c5-104">Zkontrolujte stav své domény na [portálu Azure](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="d49c5-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="d49c5-105">Ujistěte se, že je k dispozici platné předplatné Azure AD a že služby Azure AD Domain Services jsou povolené.</span><span class="sxs-lookup"><span data-stu-id="d49c5-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="d49c5-106">Certifikát potřebný k povolení zabezpečeného protokolu LDAP musí být získaný od důvěryhodné veřejné certifikační autority nebo může být certifikát podepsaný svým držitelem.</span><span class="sxs-lookup"><span data-stu-id="d49c5-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="d49c5-107">Ujistěte se, že certifikát splňuje požadovaná [pravidla](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="d49c5-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="d49c5-108">**Neplatný certifikát**</span><span class="sxs-lookup"><span data-stu-id="d49c5-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="d49c5-109">Pokud chcete certifikát obnovit, postupujte podle pokynů k vytvoření nového certifikátu a opětovném nahrání: [nakonfigurujte protokol LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d49c5-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="d49c5-110">Informace o řešení známých problémů se zabezpečenými upozorněními LDAP v Azure Active Directory Domain Services najdete v článku [řešení upozornění LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d49c5-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
