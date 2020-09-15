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
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="9447a-102">Vyprší platnost federačního certifikátu služby AD FS</span><span class="sxs-lookup"><span data-stu-id="9447a-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="9447a-103">Tento problém vyřešíte takto:</span><span class="sxs-lookup"><span data-stu-id="9447a-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="9447a-104">Nainstalujte modul Microsoft Azure Active Directory pro Windows PowerShell do počítače (Pokud modul ještě není nainstalovaný).</span><span class="sxs-lookup"><span data-stu-id="9447a-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="9447a-105">Přejděte na [Správa Azure AD pomocí Windows PowerShellu](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="9447a-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="9447a-106">Postupujte podle kroků uvedených v části scénář 1: platnost podpisového certifikátu tokenu služby AD FS v části ["při přihlašování federovaného uživatele do Microsoft 365, Azure nebo Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)došlo k chybě při přístupu k webu.</span><span class="sxs-lookup"><span data-stu-id="9447a-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="9447a-107">Postupujte podle pokynů v tématu [aktualizace nebo oprava nastavení federované domény v Microsoft, Azure nebo Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="9447a-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="9447a-108">Další informace o prodloužení federačních certifikátů najdete v článku [obnovení federačních certifikátů pro Microsoft 365 a Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="9447a-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
