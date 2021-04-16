---
title: Platnost jednoho z místních certifikátů služby Federation Service vyprší
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810045"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Platnost jednoho z místních certifikátů služby Federation Service vyprší

Tento problém vyřešíte takto:
  
- Nainstalujte modul Microsoft Azure Active Directory pro Windows PowerShell na počítač (pokud ještě není nainstalovaný). Pokud to chcete udělat, přejděte na [Azure Active Directory PowerShell pro Graph. ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Pokud se federovaný uživatel přihlásí k [Microsoftu 365, Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)nebo Intune, postupujte podle pokynů v části Scénář 1: Platnost podpisového certifikátu tokenu služby AD FS vypršela.
    
- Postupujte podle pokynů v článku Jak aktualizovat nebo opravit nastavení federované domény v [Microsoftu 365, Azure nebo Intune.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)
    
Další informace o prodlužování certifikátů federace najdete v článku [Prodloužení certifikátů pro O365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)a Azure AD .
  

