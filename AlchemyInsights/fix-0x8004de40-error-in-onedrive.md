---
title: Oprava 0x8004de40 v OneDrivu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649741"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="80495-102">Oprava 0x8004de40 v OneDrivu</span><span class="sxs-lookup"><span data-stu-id="80495-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="80495-103">Pokud používáte Windows 7 a zobrazí se tato chyba, aktualizujte protokol [TLS 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)jako výchozí zabezpečené protokoly ve WinHTTP ve Windows .</span><span class="sxs-lookup"><span data-stu-id="80495-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="80495-104">Pokud používáte Windows 10 a na OneDrivu se zobrazí 0x8004de40 chyba:</span><span class="sxs-lookup"><span data-stu-id="80495-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="80495-105">Restartujte ovlivněný počítač při připojení k doméně adresáře Acitve.</span><span class="sxs-lookup"><span data-stu-id="80495-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="80495-106">Pokud restartování problém nevyřeší, odpojte se a znovu se ke svému zařízení připojíte z Azure AD.</span><span class="sxs-lookup"><span data-stu-id="80495-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="80495-107">**Poznámka:** Při provádění těchto kroků byste měli být v podnikové síti.</span><span class="sxs-lookup"><span data-stu-id="80495-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="80495-108">Tyto kroky nedělejte, když nejste připojení ke své podnikové infrastruktuře (například na cestách).</span><span class="sxs-lookup"><span data-stu-id="80495-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="80495-109">Otevřete příkazový řádek se zvýšenými oprávněními tak, že **vyberete Start,** klikněte pravým tlačítkem myši na **Příkazový řádek** a pak vyberte **Spustit jako správce.**</span><span class="sxs-lookup"><span data-stu-id="80495-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="80495-110">Zadejte *dsregcmd /leave a* stiskněte **Enter.**</span><span class="sxs-lookup"><span data-stu-id="80495-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="80495-111">Po dokončení zadejte *dsregcmd /join* a stiskněte **Enter.**</span><span class="sxs-lookup"><span data-stu-id="80495-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="80495-112">Po dokončení zavřete příkazový řádek.</span><span class="sxs-lookup"><span data-stu-id="80495-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="80495-113">Restartujte počítač a přihlaste se k OneDrivu.</span><span class="sxs-lookup"><span data-stu-id="80495-113">Reboot the computer, and log into OneDrive.</span></span>