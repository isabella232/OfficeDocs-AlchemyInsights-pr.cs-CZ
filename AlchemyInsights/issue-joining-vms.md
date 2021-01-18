---
title: Problém při připojování k VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884979"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="27da2-102">Problém při připojování k VMs</span><span class="sxs-lookup"><span data-stu-id="27da2-102">Issue joining VMs</span></span>

<span data-ttu-id="27da2-103">Pokud chcete vyřešit problémy, ke kterým dochází při připojování k virtuálním počítači, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="27da2-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="27da2-104">Zkuste se přihlásit pomocí formátu **UPN** (například ' joeuser@contoso.com ') místo formátu **sAMAccountName** (' CONTOSO\joeuser ').</span><span class="sxs-lookup"><span data-stu-id="27da2-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="27da2-105">Ujistěte se, že jste v souladu s postupem uvedeným v příručce *Začínáme* zapnutou funkci Synchronizace hesel.</span><span class="sxs-lookup"><span data-stu-id="27da2-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="27da2-106">Zkontrolujte, že daný uživatelský účet není externí účet v Azure AD.</span><span class="sxs-lookup"><span data-stu-id="27da2-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="27da2-107">Externí uživatelé se nemohou přihlásit ke spravované doméně, protože doménové služby Azure AD neobsahují přihlašovací údaje těchto uživatelských účtů.</span><span class="sxs-lookup"><span data-stu-id="27da2-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="27da2-108">Pokud je ovlivněný uživatelský účet jenom Cloud, ujistěte se, že uživatelé změnili své heslo po tom, co jste povolili služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="27da2-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="27da2-109">Tento krok způsobí vygenerování hodnot hash přihlašovacích údajů pro služby domény Azure AD.</span><span class="sxs-lookup"><span data-stu-id="27da2-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="27da2-110">Pokud se příslušné uživatelské účty synchronizují z místního adresáře, zkontrolujte, že je nakonfigurovaná doporučená verze Azure AD Connect, která provádí úplnou synchronizaci.</span><span class="sxs-lookup"><span data-stu-id="27da2-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="27da2-111">Pokud problémy přetrvávají po potvrzení kroku 4, proveďte z synchronizačního počítače následující příkazy:</span><span class="sxs-lookup"><span data-stu-id="27da2-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="27da2-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="27da2-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>