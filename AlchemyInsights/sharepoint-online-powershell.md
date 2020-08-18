---
title: PowerShell SharePointu Online
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786882"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="9928a-102">PowerShell SharePointu Online</span><span class="sxs-lookup"><span data-stu-id="9928a-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="9928a-103">Pracujete s PowerShellem nebo skripty v SharePointu Online?</span><span class="sxs-lookup"><span data-stu-id="9928a-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="9928a-104">Další informace najdete v následujících odkazech.</span><span class="sxs-lookup"><span data-stu-id="9928a-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="9928a-105">Začínáme s prostředím SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="9928a-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="9928a-106">Připojení k SPO PowerShellu s vícefaktorového ověřováním (MFA)</span><span class="sxs-lookup"><span data-stu-id="9928a-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="9928a-107">[Vzory a postupy služby SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) obsahují knihovnu příkazů PowerShellu, která umožňuje provádět složité akce správy ke spo.</span><span class="sxs-lookup"><span data-stu-id="9928a-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="9928a-108">Pokud máte problémy s připojením pomocí prostředí SPO Management Shell, ujistěte se, že jste aktualizovali nejnovější verzi, a zkuste [modul importovat znovu](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) pomocí *modulu import – Microsoft. online. SharePoint. PowerShell* .</span><span class="sxs-lookup"><span data-stu-id="9928a-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="9928a-109">Pokud zkoušíte spustit skripty objektového modelu na straně klienta, budete muset mít na místním počítači nainstalovanou [sadu SDK součástí klienta SharePointu Online](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="9928a-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="9928a-110">Pokud máte problémy se spouštěním skriptů z PowerShellu, můžete zvážit, že se PowerShell spouští jako správce a změní se [zásady spuštění](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="9928a-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>