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
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="a28ee-102">Vypršení náječí federačního certifikátu ADFS</span><span class="sxs-lookup"><span data-stu-id="a28ee-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="a28ee-103">Tento problém vyřešíte takto:</span><span class="sxs-lookup"><span data-stu-id="a28ee-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="a28ee-104">Nainstalujte modul Microsoft Azure Active Directory pro Windows PowerShell na počítač (pokud ještě není nainstalovaný).</span><span class="sxs-lookup"><span data-stu-id="a28ee-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="a28ee-105">Pokud to chcete udělat, přejděte na [Spravovat Azure AD pomocí Windows PowerShellu.](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="a28ee-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="a28ee-106">Pokud se federovaný uživatel přihlásí k [Microsoftu 365, Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)nebo Intune, postupujte podle pokynů v části Scénář 1: Platnost podpisového certifikátu tokenu služby AD FS vypršela.</span><span class="sxs-lookup"><span data-stu-id="a28ee-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="a28ee-107">Postupujte podle pokynů v článku Aktualizace nebo oprava nastavení federované domény v [Microsoftu, Azure](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)nebo Intune.</span><span class="sxs-lookup"><span data-stu-id="a28ee-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="a28ee-108">Další informace o prodlužování certifikátů federace najdete v článku Prodloužení federačních certifikátů [pro Microsoft 365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)a Azure Active Directory .</span><span class="sxs-lookup"><span data-stu-id="a28ee-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
