---
title: Vyprší platnost jednoho z místních certifikátů služby Federation Service
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673490"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Vyprší platnost jednoho z místních certifikátů služby Federation Service

Tento problém vyřešíte takto:
  
- Nainstalujte modul Microsoft Azure Active Directory pro Windows PowerShell do počítače (Pokud modul ještě není nainstalovaný). K tomu použijte [PowerShell služby Azure Active Directory pro graf](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) .
    
- Postupujte podle kroků uvedených v části scénář 1: platnost podpisového certifikátu tokenu služby AD FS v části ["při přihlašování federovaného uživatele do Microsoft 365, Azure nebo Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)došlo k chybě při přístupu k webu.
    
- Postupujte podle pokynů v tématu [aktualizace nebo oprava nastavení federované domény v Microsoft 365, Azure nebo Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Další informace o obnovení federačních certifikátů najdete v tématu [obnovení certifikátu pro O365 a Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

