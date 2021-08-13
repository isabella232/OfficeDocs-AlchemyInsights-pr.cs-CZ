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
ms.openlocfilehash: d0658b05b81ac45e7ce80323ad29898599482c4d3430d886627af6e9f8d136f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53985210"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Platnost jednoho z místních certifikátů služby Federation Service vyprší

Tento problém vyřešíte takto:
  
- Nainstalujte Microsoft Azure Active Directory modul pro Windows PowerShell počítače (pokud ještě není nainstalovaný). Pokud to chcete udělat, přejděte [na Azure Active Directory PowerShellu pro Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Postupujte podle pokynů v části "Scénář 1: Platnost podpisového certifikátu tokenu služby AD FS vypršela" chyby "Došlo k problému s přístupem k webu" ze služby AD FS, když se federovaný uživatel přihlásí k [Microsoft 365, Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)nebo Intune .
    
- Postupujte podle pokynů v tématu Jak aktualizovat nebo opravit nastavení federované domény v [Microsoft 365, Azure nebo Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Další informace o prodlužování certifikátů federace najdete v článku [Prodloužení certifikátů pro O365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)a Azure AD .
  

