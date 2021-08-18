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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090405"
---
# <a name="configure-ldap"></a>Konfigurace protokolu LDAP

Pokud chcete nakonfigurovat LDAP, proveďte následující kroky:

1. Zkontrolujte stav vaší domény na [portálu Azure Portal](https://aka.ms/aadds-health).
1. Ujistěte se, že je dostupné platné předplatné Azure AD a že je služba Azure AD Domain Services povolená.
1. Certifikát potřebný k povolení zabezpečeného protokolu LDAP musí být získán od důvěryhodné veřejné certifikační autority nebo musí být certifikát podepsaný svým držitelem.
1. Ujistěte se, že certifikát dodržuje požadované [pokyny](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Neplatný certifikát**
1. Pokud chcete certifikát obnovit, postupujte podle pokynů k vytvoření nového certifikátu a reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Pokud chcete vyřešit známý problém se zabezpečenými výstrahami LDAP ve službě Azure Active Directory Domain Services, podívejte se na téma [Řešení upozornění LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
