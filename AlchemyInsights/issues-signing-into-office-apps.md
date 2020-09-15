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
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695172"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="0d6fd-102">Oprava aplikací Microsoft 365 "důvěryhodný čip TPM vašeho počítače nefunguje správně" zpráva</span><span class="sxs-lookup"><span data-stu-id="0d6fd-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="0d6fd-103">Pokud chcete tuto chybu vyřešit, vyzkoušejte následující:</span><span class="sxs-lookup"><span data-stu-id="0d6fd-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="0d6fd-104">Nainstalujte si nejnovější aktualizace pro [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="0d6fd-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="0d6fd-105">Pomocí Správce přihlašovacích údajů systému Windows [vymažte přihlašovací údaje Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .</span><span class="sxs-lookup"><span data-stu-id="0d6fd-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="0d6fd-106">**Poznámka:** Cesty registru pro Office 2016 se změnily na 16,0.</span><span class="sxs-lookup"><span data-stu-id="0d6fd-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="0d6fd-107">(Např.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="0d6fd-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="0d6fd-108">Zkuste [obnovit](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) chyby čipu TPM (Trusted Platform Module).</span><span class="sxs-lookup"><span data-stu-id="0d6fd-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="0d6fd-109">Nastavte EnableADAL = 0 pomocí následujících kroků:</span><span class="sxs-lookup"><span data-stu-id="0d6fd-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="0d6fd-110">Klikněte pravým tlačítkem myši na tlačítko Start systému Windows, zvolte **Spustit**, zadejte **Regedit**a pak zvolte **OK**.</span><span class="sxs-lookup"><span data-stu-id="0d6fd-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="0d6fd-111">Výběrem možnosti **Ano** povolíte, aby Editor registru prováděl v zařízení změny.</span><span class="sxs-lookup"><span data-stu-id="0d6fd-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="0d6fd-112">V editoru registru přidejte hodnotu DWORD pro **EnableADAL** s nastavením **0** v části HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="0d6fd-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="0d6fd-113">Další informace najdete v článku [problémy s připojením při přihlášení po aktualizaci na Office 2016 Build 16.0.7967 ve Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="0d6fd-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>