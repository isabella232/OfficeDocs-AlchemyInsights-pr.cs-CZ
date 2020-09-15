---
title: Vyprší platnost federačního certifikátu služby AD FS
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686707"
---
# <a name="adfs-federation-certificate-expiring"></a>Vyprší platnost federačního certifikátu služby AD FS

Tento problém vyřešíte takto:
  
1. Nainstalujte modul Microsoft Azure Active Directory pro Windows PowerShell do počítače (Pokud modul ještě není nainstalovaný). Přejděte na [Správa Azure AD pomocí Windows PowerShellu](https://aka.ms/aadposh).

2. Postupujte podle kroků uvedených v části scénář 1: platnost podpisového certifikátu tokenu služby AD FS v části ["při přihlašování federovaného uživatele do Microsoft 365, Azure nebo Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)došlo k chybě při přístupu k webu.

3. Postupujte podle pokynů v tématu [aktualizace nebo oprava nastavení federované domény v Microsoft, Azure nebo Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Další informace o prodloužení federačních certifikátů najdete v článku [obnovení federačních certifikátů pro Microsoft 365 a Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
