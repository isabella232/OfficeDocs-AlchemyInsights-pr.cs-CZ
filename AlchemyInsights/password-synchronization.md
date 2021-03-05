---
title: Synchronizace hesel
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481143"
---
# <a name="password-synchronization"></a><span data-ttu-id="5f273-102">Synchronizace hesel</span><span class="sxs-lookup"><span data-stu-id="5f273-102">Password synchronization</span></span>

<span data-ttu-id="5f273-103">**Synchronizace hodnot hash hesel nefunguje vůbec.**</span><span class="sxs-lookup"><span data-stu-id="5f273-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="5f273-104">K některým běžným problémům, se kterými se zákazníci setkávají, když synchronizace hodnot hash hesel nefunguje, jsou:</span><span class="sxs-lookup"><span data-stu-id="5f273-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="5f273-105">Účet služby Active Directory používaný službou Azure AD Connect ke  komunikaci s místní  službou Active Directory nemá udělená oprávnění Replikovat změny adresáře a Replikovat změny adresáře – všechna oprávnění, která jsou potřeba pro synchronizaci hesel – musíte to vyřešit udělením těchto oprávnění účtu služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5f273-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="5f273-106">Synchronizace hodnot hash hesel je v průvodci Azure  AD Connect zakázaná poté, co správce změnil metodu Sign-In uživatele ze synchronizace hesel na jinou možnost, například Federování se službou **AD FS.** Můžete to vyřešit tak, že v průvodci Azure AD Connect znovu povolíte funkci synchronizace hodnot **hash** hesel.</span><span class="sxs-lookup"><span data-stu-id="5f273-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="5f273-107">Potíže s připojením k místní službě Active Directory</span><span class="sxs-lookup"><span data-stu-id="5f273-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="5f273-108">Některé řadičy domény například nejsou dostupné službou [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Azure AD Connect nebo firewall zablokuje požadované porty – musíte to opravit tím, že zajistíte správné propojení mezi serverem Azure AD Connect a místní službou Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5f273-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="5f273-109">Server Azure AD Connect právě pracuje v režimu konfigurace, což by vedlo k tomu, že server nebude moct používat a hash hesel – pokud chcete tento problém vyřešit, postupujte podle kroků popsaných v části Řešení problémů se synchronizací hesel se synchronizací Azure AD Connect – žádná hesla se [synchronizují.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="5f273-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="5f273-110">**Některým uživatelům nefunguje synchronizace hodnot hash hesel**</span><span class="sxs-lookup"><span data-stu-id="5f273-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="5f273-111">Pokud jste zjistili, že se hodnota hash  hesel pro uživatele nesynchronuje, použijte k prozkoumání a vyřešení problému úlohu řešení potíží v Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5f273-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="5f273-112">Proveďte následující úkoly:</span><span class="sxs-lookup"><span data-stu-id="5f273-112">Perform the following tasks:</span></span>

    <span data-ttu-id="5f273-113">a.</span><span class="sxs-lookup"><span data-stu-id="5f273-113">a.</span></span> [<span data-ttu-id="5f273-114">Spuštění úkolu pro řešení potíží v průvodci</span><span class="sxs-lookup"><span data-stu-id="5f273-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="5f273-115">b.</span><span class="sxs-lookup"><span data-stu-id="5f273-115">b.</span></span> [<span data-ttu-id="5f273-116">Prozkoumejte problém se synchronizací hodnot hash hesel pro konkrétní použití pomocí rutiny pro řešení potíží.</span><span class="sxs-lookup"><span data-stu-id="5f273-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="5f273-117">Pro uživatele je povolený objekt místního uživatele služby Active Directory, musí **při** příštím přihlášení změnit heslo.</span><span class="sxs-lookup"><span data-stu-id="5f273-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="5f273-118">Pokud je tato možnost povolená, přiřadí se uživateli dočasné heslo a při dalším přihlášení se zobrazí výzva ke změně hesla.</span><span class="sxs-lookup"><span data-stu-id="5f273-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="5f273-119">Azure AD Connect nesynchronuje dočasná hesla se službou Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5f273-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="5f273-120">Pokud chcete vyřešit výše uvedený problém, proveďte jednu z následujících akcí:</span><span class="sxs-lookup"><span data-stu-id="5f273-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="5f273-121">Požádejte uživatele, aby se přihlašuje k místní aplikaci (třeba ke stolnímu počítači s Windows) a změnil heslo.</span><span class="sxs-lookup"><span data-stu-id="5f273-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="5f273-122">Nové heslo se synchronizuje s Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5f273-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="5f273-123">Správce musí aktualizovat heslo uživatele, aniž by povolili možnost Uživatel musí při příštím přihlášení změnit heslo a nové heslo sdílet s uživatelem.</span><span class="sxs-lookup"><span data-stu-id="5f273-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="5f273-124">Místní objekt uživatele služby Active Directory **není** správně nakonfigurovaný na synchronizaci objektů nebo synchronizaci hesla.</span><span class="sxs-lookup"><span data-stu-id="5f273-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="5f273-125">Pokud chcete tento problém vyřešit, postupujte podle kroků popsaných v tématu Řešení potíží se synchronizací hodnot hash hesel [se synchronizací Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="5f273-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







