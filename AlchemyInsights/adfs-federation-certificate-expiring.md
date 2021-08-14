---
title: Vypršení náječí federačního certifikátu ADFS
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952962"
---
# <a name="adfs-federation-certificate-expiring"></a>Vypršení náječí federačního certifikátu ADFS

Tento problém vyřešíte takto:
  
1. Nainstalujte Microsoft Azure Active Directory modul pro Windows PowerShell počítače (pokud ještě není nainstalovaný). Pokud to chcete udělat, přejděte na [Spravovat Azure AD pomocí Windows PowerShell](https://aka.ms/aadposh).

2. Postupujte podle pokynů v části "Scénář 1: Platnost podpisového certifikátu tokenu služby AD FS vypršela" chyby "Došlo k problému s přístupem k webu" ze služby AD FS, když se federovaný uživatel přihlásí k [Microsoft 365, Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)nebo Intune .

3. Postupujte podle pokynů v článku Aktualizace nebo oprava nastavení federované domény v [Microsoftu, Azure](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)nebo Intune.

    Další informace o prodlužování certifikátů federace najdete v tématu Prodloužení federačních certifikátů pro Microsoft 365 a [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
