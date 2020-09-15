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
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="fcdb6-102">Vyprší platnost jednoho z místních certifikátů služby Federation Service</span><span class="sxs-lookup"><span data-stu-id="fcdb6-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="fcdb6-103">Tento problém vyřešíte takto:</span><span class="sxs-lookup"><span data-stu-id="fcdb6-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="fcdb6-104">Nainstalujte modul Microsoft Azure Active Directory pro Windows PowerShell do počítače (Pokud modul ještě není nainstalovaný).</span><span class="sxs-lookup"><span data-stu-id="fcdb6-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="fcdb6-105">K tomu použijte [PowerShell služby Azure Active Directory pro graf](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) .</span><span class="sxs-lookup"><span data-stu-id="fcdb6-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="fcdb6-106">Postupujte podle kroků uvedených v části scénář 1: platnost podpisového certifikátu tokenu služby AD FS v části ["při přihlašování federovaného uživatele do Microsoft 365, Azure nebo Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)došlo k chybě při přístupu k webu.</span><span class="sxs-lookup"><span data-stu-id="fcdb6-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="fcdb6-107">Postupujte podle pokynů v tématu [aktualizace nebo oprava nastavení federované domény v Microsoft 365, Azure nebo Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="fcdb6-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="fcdb6-108">Další informace o obnovení federačních certifikátů najdete v tématu [obnovení certifikátu pro O365 a Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="fcdb6-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

