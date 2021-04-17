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
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821944"
---
# <a name="adfs-federation-certificate-expiring"></a>Vypršení náječí federačního certifikátu ADFS

Tento problém vyřešíte takto:
  
1. Nainstalujte modul Microsoft Azure Active Directory pro Windows PowerShell na počítač (pokud ještě není nainstalovaný). Pokud to chcete udělat, přejděte na [Spravovat Azure AD pomocí Windows PowerShellu.](https://aka.ms/aadposh)

2. Pokud se federovaný uživatel přihlásí k [Microsoftu 365, Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)nebo Intune, postupujte podle pokynů v části Scénář 1: Platnost podpisového certifikátu tokenu služby AD FS vypršela.

3. Postupujte podle pokynů v článku Aktualizace nebo oprava nastavení federované domény v [Microsoftu, Azure](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)nebo Intune.

    Další informace o prodlužování certifikátů federace najdete v článku Prodloužení federačních certifikátů [pro Microsoft 365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)a Azure Active Directory .
