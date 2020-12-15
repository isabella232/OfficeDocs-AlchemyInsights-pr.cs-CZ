---
title: Automatické přihlášení k Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676966"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="beb59-102">Automatické přihlášení k Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="beb59-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="beb59-103">Microsoft Edge používá výchozí účet operačního systému k automatickému přihlášení uživatele podle toho, jak je nastavené zařízení uživatele.</span><span class="sxs-lookup"><span data-stu-id="beb59-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="beb59-104">Tady jsou popsané scénáře jednotlivých typů konfigurací zařízení a jeho proces přihlašování závislým uživatelem:</span><span class="sxs-lookup"><span data-stu-id="beb59-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="beb59-105">**Zařízení je hybridní/AAD-J**: Tato možnost je k dispozici ve Windows 10, Windows pro nižší verzi a v odpovídajících serverových verzích.</span><span class="sxs-lookup"><span data-stu-id="beb59-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="beb59-106">Uživatelé se automaticky přihlásí pomocí svých účtů služby Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="beb59-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="beb59-107">**Zařízení je spojené s doménou**: Tato možnost je k dispozici ve Windows 10, Windows pro nižší úrovni a v odpovídajících serverových verzích.</span><span class="sxs-lookup"><span data-stu-id="beb59-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="beb59-108">Ve výchozím nastavení nejsou uživatelé s účty domény automaticky přihlášeni. Pokud chcete povolit automatické přihlašování, použijte zásady **ConfigureOnPremisesAccountAutoSignIn** .</span><span class="sxs-lookup"><span data-stu-id="beb59-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="beb59-109">Pokud chcete povolit automatické přihlašování pro uživatele s účty Azure AD, zvažte hybridní připojení svých zařízení.</span><span class="sxs-lookup"><span data-stu-id="beb59-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="beb59-110">**Výchozím účtem operačního systému je účet Microsoft**: Tato možnost je dostupná ve Windows 10 RS3 (verze 1709, Build 10.0.16299) a novější verze.</span><span class="sxs-lookup"><span data-stu-id="beb59-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="beb59-111">U podnikových zařízení se nepravděpodobná situace.</span><span class="sxs-lookup"><span data-stu-id="beb59-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="beb59-112">Pokud je ale výchozím účtem operačního systému účet Microsoft, Microsoft Edge ho automaticky přihlásí pomocí účtu Microsoft.</span><span class="sxs-lookup"><span data-stu-id="beb59-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
