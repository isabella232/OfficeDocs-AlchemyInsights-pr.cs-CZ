---
title: Přihlášení do Windows 10 bez použití hesla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719946"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="e9514-102">Přihlášení do Windows 10 bez použití hesla</span><span class="sxs-lookup"><span data-stu-id="e9514-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="e9514-103">Chcete-li se vyhnout zadávání hesla při spuštění systému Windows, doporučujeme použít jednu z možností zabezpečeného přihlášení Windows Hello, jako je PIN, rozpoznávání obličeje nebo otisk prstu, pokud je dostupný.</span><span class="sxs-lookup"><span data-stu-id="e9514-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="e9514-104">Pokud opravdu chcete zakázat zabezpečené přihlašování, přečtěte si následující pokyny v části Automatické přihlášení k Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e9514-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="e9514-105">**Zabezpečení alternativních možností Windows Hello s heslem účtu**</span><span class="sxs-lookup"><span data-stu-id="e9514-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="e9514-106">Přejděte na **nastavení > účty > možnosti přihlášení** (nebo klikněte [sem](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="e9514-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="e9514-107">Budou dostupné možnosti přihlášení.</span><span class="sxs-lookup"><span data-stu-id="e9514-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="e9514-108">Příklad:</span><span class="sxs-lookup"><span data-stu-id="e9514-108">For example:</span></span>

![Možnosti přihlášení](media/sign-in-options.png)

<span data-ttu-id="e9514-110">Kliknutím nebo klepnutím na jednu z možností ji nakonfigurujte.</span><span class="sxs-lookup"><span data-stu-id="e9514-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="e9514-111">Při příštím spuštění nebo odemčení Windows budete moct místo hesla použít novou možnost.</span><span class="sxs-lookup"><span data-stu-id="e9514-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="e9514-112">**Automatické přihlášení do Windows 10**</span><span class="sxs-lookup"><span data-stu-id="e9514-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="e9514-113">**Poznámka**: automatické přihlašování je vhodné, ale představuje bezpečnostní riziko, obzvláště v případě, že je váš počítač přístupný více lidem.</span><span class="sxs-lookup"><span data-stu-id="e9514-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="e9514-114">Klikněte nebo klepněte na tlačítko **Start** na hlavním panelu.</span><span class="sxs-lookup"><span data-stu-id="e9514-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="e9514-115">Zadejte **netplwiz** a stisknutím klávesy ENTER otevřete okno uživatelské účty.</span><span class="sxs-lookup"><span data-stu-id="e9514-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="e9514-116">V části **uživatelské účty**klikněte na účet, ke kterému se chcete automaticky přihlásit při spuštění systému Windows.</span><span class="sxs-lookup"><span data-stu-id="e9514-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="e9514-117">Zrušte zaškrtnutí políčka před použitím tohoto počítače musí uživatelé zadat uživatelské jméno a heslo.</span><span class="sxs-lookup"><span data-stu-id="e9514-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Uživatelé musí zadat uživatelské jméno a heslo.](media/users-must-enter-username.png)

5. <span data-ttu-id="e9514-119">Klikněte na tlačítko **OK**.</span><span class="sxs-lookup"><span data-stu-id="e9514-119">Click **OK**.</span></span> <span data-ttu-id="e9514-120">Zobrazí se výzva k zadání a potvrzení hesla vybraného účtu.</span><span class="sxs-lookup"><span data-stu-id="e9514-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="e9514-121">Kliknutím na **OK** dokončete.</span><span class="sxs-lookup"><span data-stu-id="e9514-121">Click **OK** to finish.</span></span> <span data-ttu-id="e9514-122">Po příštím spuštění Windows 10 se automaticky přihlásí k vybranému účtu.</span><span class="sxs-lookup"><span data-stu-id="e9514-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
