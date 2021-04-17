---
title: Přihlášení k Windows 10 bez použití hesla
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830539"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="052e0-102">Přihlášení k Windows 10 bez použití hesla</span><span class="sxs-lookup"><span data-stu-id="052e0-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="052e0-103">Abyste při spuštění Windows museli zapisovat heslo, doporučujeme použít jednu z možností zabezpečeného přihlášení k Windows Hello, například PIN kód, rozpoznávání obličeje nebo otisk prstu, pokud je k dispozici.</span><span class="sxs-lookup"><span data-stu-id="052e0-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="052e0-104">Pokud opravdu chcete zakázat zabezpečené přihlášení, přečtěte si níže uvedené pokyny k automatickému přihlášení k Windows 10.</span><span class="sxs-lookup"><span data-stu-id="052e0-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="052e0-105">**Zabezpečení alternativ k hesly účtu ve Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="052e0-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="052e0-106">Přejděte na **Nastavení > Účty > možnosti přihlášení** (nebo klikněte [sem).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="052e0-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="052e0-107">Zobrazí se dostupné možnosti přihlášení.</span><span class="sxs-lookup"><span data-stu-id="052e0-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="052e0-108">Příklad:</span><span class="sxs-lookup"><span data-stu-id="052e0-108">For example:</span></span>

![Možnosti přihlášení](media/sign-in-options.png)

<span data-ttu-id="052e0-110">Klikněte nebo klepněte na jednu z možností konfigurace.</span><span class="sxs-lookup"><span data-stu-id="052e0-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="052e0-111">Až příště spustíte nebo odemknete Windows, budete moct místo hesla použít novou možnost.</span><span class="sxs-lookup"><span data-stu-id="052e0-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="052e0-112">**Automatické přihlášení k Windows 10**</span><span class="sxs-lookup"><span data-stu-id="052e0-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="052e0-113">**Poznámka:** Automatické přihlašování je pohodlné, ale představuje bezpečnostní riziko, zejména pokud je váš počítač přístupný více lidmi.</span><span class="sxs-lookup"><span data-stu-id="052e0-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="052e0-114">Klikněte nebo klepněte **na tlačítko Start** na hlavním panelu.</span><span class="sxs-lookup"><span data-stu-id="052e0-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="052e0-115">Zadejte **netplwiz** a stisknutím klávesy Enter otevřete okno Uživatelské účty.</span><span class="sxs-lookup"><span data-stu-id="052e0-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="052e0-116">V **části Uživatelské účty** klikněte na účet, ke který se chcete automaticky přihlásit při spuštění Windows.</span><span class="sxs-lookup"><span data-stu-id="052e0-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="052e0-117">Zrušte zaškrtnutí políčka Uživatelé musí zadat uživatelské jméno a heslo pro použití tohoto počítače.</span><span class="sxs-lookup"><span data-stu-id="052e0-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Uživatelé musí zadat možnost uživatelského jména a hesla.](media/users-must-enter-username.png)

5. <span data-ttu-id="052e0-119">Klikněte na tlačítko **OK**.</span><span class="sxs-lookup"><span data-stu-id="052e0-119">Click **OK**.</span></span> <span data-ttu-id="052e0-120">Zobrazí se dotaz, jestli chcete zadat a potvrdit heslo k vybranému účtu.</span><span class="sxs-lookup"><span data-stu-id="052e0-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="052e0-121">Dokončete to kliknutím **na OK.**</span><span class="sxs-lookup"><span data-stu-id="052e0-121">Click **OK** to finish.</span></span> <span data-ttu-id="052e0-122">Při příštím spuštění Windows 10 se automaticky přihlásí k vybranému účtu.</span><span class="sxs-lookup"><span data-stu-id="052e0-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
