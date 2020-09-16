---
title: Nastavení automatických odpovědí pro poštovní schránku
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 03c530e7ce5f00fce2222cf9993930b97e5a2818
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715122"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="1ea40-102">Nastavení automatických odpovědí pro poštovní schránku uživatele</span><span class="sxs-lookup"><span data-stu-id="1ea40-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="1ea40-103">**Metoda 1**</span><span class="sxs-lookup"><span data-stu-id="1ea40-103">**Method 1**</span></span>

1. <span data-ttu-id="1ea40-104">Přihlaste se na portál Microsoftu 365.</span><span class="sxs-lookup"><span data-stu-id="1ea40-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="1ea40-105">Přejděte na **Uživatelé > Aktivní uživatelé** (nebo **Skupiny > Sdílené poštovní schránky**, pokud nastavujete sdílenou poštovní schránku).</span><span class="sxs-lookup"><span data-stu-id="1ea40-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="1ea40-106">Vyberte uživatele, který má poštovní schránku Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="1ea40-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="1ea40-107">V rozevírací nabídce vpravo přejděte na **Nastavení pošty > Automatické odpovědi** (pokud se jedná o sdílenou poštovní schránku, stačí v rozevírací nabídce kliknout na **Automatické odpovědi**).</span><span class="sxs-lookup"><span data-stu-id="1ea40-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="1ea40-108">**Metoda 2**</span><span class="sxs-lookup"><span data-stu-id="1ea40-108">**Method 2**</span></span>

1. <span data-ttu-id="1ea40-109">Přihlaste se k portálu pro správu Microsoftu 365 pomocí přihlašovacích údajů správce.</span><span class="sxs-lookup"><span data-stu-id="1ea40-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="1ea40-110">Rozbalte **Centra pro správu** a pak klikněte na **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="1ea40-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="1ea40-111">V pravém horním rohu klikněte na obrázek, klikněte na **Jiný uživatel** a vyberte poštovní schránku uživatele, kterou chcete změnit.</span><span class="sxs-lookup"><span data-stu-id="1ea40-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="1ea40-112">Na levé straně vyberte **Možnosti**, klikněte na **Uspořádat e-mail** a pak klikněte na **Automatické odpovědi**.</span><span class="sxs-lookup"><span data-stu-id="1ea40-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="1ea40-113">**Metoda 3**</span><span class="sxs-lookup"><span data-stu-id="1ea40-113">**Method 3**</span></span>

<span data-ttu-id="1ea40-114">Spusťte v Exchange Online PowerShellu tuto rutinu:</span><span class="sxs-lookup"><span data-stu-id="1ea40-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="1ea40-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="1ea40-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="1ea40-116">Další informace o této rutině najdete v tématu [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="1ea40-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
