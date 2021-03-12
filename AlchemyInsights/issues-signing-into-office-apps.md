---
title: Problémy s přihlášením k aplikacím Microsoft 365
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
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709099"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="eb8d3-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is notfunctioning properly" message</span><span class="sxs-lookup"><span data-stu-id="eb8d3-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="eb8d3-103">Pokud chcete tuto chybu vyřešit, vyzkoušejte následující:</span><span class="sxs-lookup"><span data-stu-id="eb8d3-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="eb8d3-104">Nainstalujte nejnovější aktualizace [pro Windows a](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="eb8d3-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="eb8d3-105">[Vymažte přihlašovací údaje Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) pomocí Správce přihlašovacích údajů systému Windows.</span><span class="sxs-lookup"><span data-stu-id="eb8d3-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="eb8d3-106">**Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0.</span><span class="sxs-lookup"><span data-stu-id="eb8d3-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="eb8d3-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="eb8d3-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="eb8d3-108">Zkuste [chyby MODULU](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) DŮVĚRYHODNÉ PLATFORMY (MODULEM) opravit procesem obnovení uživatele.</span><span class="sxs-lookup"><span data-stu-id="eb8d3-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="eb8d3-109">Nastavte enableADAL = 0 pomocí následujících kroků:</span><span class="sxs-lookup"><span data-stu-id="eb8d3-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="eb8d3-110">Klikněte pravým tlačítkem myši na tlačítko Start systému Windows, zvolte **Spustit,** zadejte **regedit** a pak zvolte **OK.**</span><span class="sxs-lookup"><span data-stu-id="eb8d3-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="eb8d3-111">Výběrem **možnosti** Ano povolíte Editoru registru dělat změny na vašem zařízení.</span><span class="sxs-lookup"><span data-stu-id="eb8d3-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="eb8d3-112">V Editoru registru přidejte hodnotu DWORD **EnableADAL** s nastavením **0** v HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="eb8d3-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="eb8d3-113">Další informace najdete v článku Problémy s připojením při přihlašování po aktualizaci na [build Office 2016 16.0.7967 ve Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="eb8d3-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>