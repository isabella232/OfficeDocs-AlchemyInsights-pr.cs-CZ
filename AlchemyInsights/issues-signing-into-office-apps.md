---
title: Problémy s přihlášením k aplikacím Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579858"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="15353-102">Oprava zprávy aplikace Microsoft 365 "Modul důvěryhodné platformy vašeho počítače nefunguje správně"</span><span class="sxs-lookup"><span data-stu-id="15353-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="15353-103">Pokud chcete tuto chybu vyřešit, vyzkoušejte následující:</span><span class="sxs-lookup"><span data-stu-id="15353-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="15353-104">Nainstalujte nejnovější aktualizace pro [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="15353-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="15353-105">[Vymazání přihlašovacích údajů Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocí Správce pověření systému Windows</span><span class="sxs-lookup"><span data-stu-id="15353-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="15353-106">**Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0.</span><span class="sxs-lookup"><span data-stu-id="15353-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="15353-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="15353-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="15353-108">Zkuste [proces obnovení uživatele](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) opravit selhání modulu Důvěryhodné platformy (TPM).</span><span class="sxs-lookup"><span data-stu-id="15353-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="15353-109">PovolitADAL = 0 nastavte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="15353-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="15353-110">Klepněte pravým tlačítkem myši na tlačítko Start systému Windows, zvolte **Spustit**, zadejte **příkaz regedit**a pak zvolte **OK**.</span><span class="sxs-lookup"><span data-stu-id="15353-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="15353-111">Vyberte **Ano,** chcete-li povolit Editoru registru provádět změny v zařízení.</span><span class="sxs-lookup"><span data-stu-id="15353-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="15353-112">V Editoru registru přidejte hodnotu DWORD **enableADAL** s nastavením **0** pod položkou HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="15353-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="15353-113">Další informace najdete [v tématu Problémy s připojením při přihlášení po aktualizaci na sestavení Office 2016 16.0.7967 ve Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="15353-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>