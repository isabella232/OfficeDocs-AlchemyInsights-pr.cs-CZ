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
# <a name="configure-ldap"></a>Konfigurace protokolu LDAP

Při konfiguraci protokolu LDAP postupujte takto:

1. Zkontrolujte stav své domény na [portálu Azure](https://aka.ms/aadds-health).
1. Ujistěte se, že je k dispozici platné předplatné Azure AD a že služby Azure AD Domain Services jsou povolené.
1. Certifikát potřebný k povolení zabezpečeného protokolu LDAP musí být získaný od důvěryhodné veřejné certifikační autority nebo může být certifikát podepsaný svým držitelem.
1. Ujistěte se, že certifikát splňuje požadovaná [pravidla](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Neplatný certifikát**
1. Pokud chcete certifikát obnovit, postupujte podle pokynů k vytvoření nového certifikátu a opětovném nahrání: [nakonfigurujte protokol LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Informace o řešení známých problémů se zabezpečenými upozorněními LDAP v Azure Active Directory Domain Services najdete v článku [řešení upozornění LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
