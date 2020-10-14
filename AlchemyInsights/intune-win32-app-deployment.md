---
title: Nasazení aplikací Win32 v Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461757"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="8fd8d-102">Nasazení aplikací Win32 v Intune</span><span class="sxs-lookup"><span data-stu-id="8fd8d-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="8fd8d-103">Microsoft Intune umožňuje aplikacím Win32, včetně nejenom se službou MSI a. EXE pro nasazení na zařízení s Windows 10.</span><span class="sxs-lookup"><span data-stu-id="8fd8d-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="8fd8d-104">Použitý mechanismus nasazení vyžaduje, aby byla na cílovém zařízení přítomná rozšíření pro správu Intune.</span><span class="sxs-lookup"><span data-stu-id="8fd8d-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="8fd8d-105">Editor IME bude automaticky nainstalován jako výsledek zaměření nasazení skriptu PowerShell nebo Win32 na zařízení.</span><span class="sxs-lookup"><span data-stu-id="8fd8d-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="8fd8d-106">Existují také systémy předpokladů, které musí být splněny, aby bylo možné nasadit aplikace Win32, které zahrnují:</span><span class="sxs-lookup"><span data-stu-id="8fd8d-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="8fd8d-107">Podporované platformy: Windows 10 verze 1607 nebo novější (verze Enterprise, pro a vzdělávací organizace).</span><span class="sxs-lookup"><span data-stu-id="8fd8d-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="8fd8d-108">Podporovaná architektura: x86 a x64</span><span class="sxs-lookup"><span data-stu-id="8fd8d-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="8fd8d-109">Správa zařízení: připojení k AAD a automaticky zaregistrované (včetně připojení hybridní domény a automaticky zapsaných zásad skupiny).</span><span class="sxs-lookup"><span data-stu-id="8fd8d-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="8fd8d-110">Formát balíčku aplikace:. **intunewin**  soubor připravený nástrojem pro [přípravu obsahu Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="8fd8d-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="8fd8d-111">Kladen</span><span class="sxs-lookup"><span data-stu-id="8fd8d-111">Limitations:</span></span>
    - <span data-ttu-id="8fd8d-112">Maximální velikost: 8 GB.</span><span class="sxs-lookup"><span data-stu-id="8fd8d-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="8fd8d-113">Nepodporovaná architektura: paže.</span><span class="sxs-lookup"><span data-stu-id="8fd8d-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="8fd8d-114">Projděte si dokument "[Přidání, přiřazení a monitorování aplikace Win32 v Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)", kde najdete další informace o těchto krocích.</span><span class="sxs-lookup"><span data-stu-id="8fd8d-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="8fd8d-115">Podrobnosti o řešení potíží s nasazením aplikací v systému Windows, včetně aplikací Win32, najdete v následujících dokumentech.</span><span class="sxs-lookup"><span data-stu-id="8fd8d-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="8fd8d-116">Poradce při potížích s instalací aplikace</span><span class="sxs-lookup"><span data-stu-id="8fd8d-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="8fd8d-117">Odstraňování potíží s aplikacemi Win32</span><span class="sxs-lookup"><span data-stu-id="8fd8d-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)