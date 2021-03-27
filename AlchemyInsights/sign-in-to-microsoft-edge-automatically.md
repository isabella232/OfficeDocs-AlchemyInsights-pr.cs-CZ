---
title: Automatické přihlášení k Microsoft Edgi
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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398722"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="25f84-102">Automatické přihlášení k Microsoft Edgi</span><span class="sxs-lookup"><span data-stu-id="25f84-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="25f84-103">Microsoft Edge používá výchozí účet operačního systému k automatickému přihlášení uživatele podle toho, jak je nakonfigurované zařízení uživatele.</span><span class="sxs-lookup"><span data-stu-id="25f84-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="25f84-104">Scénáře jednotlivých typů konfigurace zařízení a procesu přihlášení závislých uživatelů jsou popsané níže:</span><span class="sxs-lookup"><span data-stu-id="25f84-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="25f84-105">**Zařízení je hybridní/AAD-J:** Tato možnost je dostupná ve Windows 10, na nižší úrovni Windows a odpovídajících serverových verzích.</span><span class="sxs-lookup"><span data-stu-id="25f84-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="25f84-106">Uživatelé se automaticky přihlášeni pomocí svých účtů Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="25f84-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="25f84-107">**Zařízení je připojené k doméně:** Tato možnost je dostupná ve Windows 10, ve Windows nižší úrovni a odpovídajících serverových verzích.</span><span class="sxs-lookup"><span data-stu-id="25f84-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="25f84-108">Ve výchozím nastavení se uživatelé s účty domény nepřichytují automaticky. pokud chcete povolit automatické přihlašování, použijte zásadu **ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="25f84-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="25f84-109">Pokud chcete povolit automatické přihlašování pro uživatele s účty Azure AD, zvažte hybridní připojení k jejich zařízením.</span><span class="sxs-lookup"><span data-stu-id="25f84-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="25f84-110">**Výchozí účet operačního** systému je účet Microsoft: Tato možnost je dostupná ve Windows 10 RS3 (verze 1709, build 10.0.16299) a novějších verzích.</span><span class="sxs-lookup"><span data-stu-id="25f84-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="25f84-111">Scénář se pravděpodobně nevyskytuje na podnikových zařízeních.</span><span class="sxs-lookup"><span data-stu-id="25f84-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="25f84-112">Pokud je ale výchozím účtem operačního systému účet Microsoft, Microsoft Edge se automaticky přihlásí k uživateli pomocí účtu Microsoft.</span><span class="sxs-lookup"><span data-stu-id="25f84-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
