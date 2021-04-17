---
title: V klientovi Teams dochází k chybám?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826264"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="326b1-102">V klientovi Teams dochází k chybám?</span><span class="sxs-lookup"><span data-stu-id="326b1-102">Teams client crashing?</span></span>

<span data-ttu-id="326b1-103">Pokud v klientovi Teams dochází k chybám, vyzkoušejte následující postup:</span><span class="sxs-lookup"><span data-stu-id="326b1-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="326b1-104">Pokud používáte desktopovou aplikaci Teams, [zkontrolujte, jestli je tato aplikace kompletně aktualizovaná](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="326b1-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="326b1-105">Ujistěte se, že jsou dostupné všechny adresy URL a rozsahy adres microsoftu [365.](https://docs.microsoft.com/microsoftteams/connectivity-issues)</span><span class="sxs-lookup"><span data-stu-id="326b1-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="326b1-106">Přihlaste se pomocí účtu správce tenanta a zkontrolujte řídicí panel [stavu služby,](https://docs.microsoft.com/office365/enterprise/view-service-health) abyste ověřili, že neexistuje žádný výpadk nebo degradace služby.</span><span class="sxs-lookup"><span data-stu-id="326b1-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="326b1-107">Odinstalace a přeinstalace aplikace Teams (odkaz)</span><span class="sxs-lookup"><span data-stu-id="326b1-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="326b1-108">Přejděte do složky %appdata%\Microsoft\teams\ na počítači a odstraňte všechny soubory v tomto adresáři.</span><span class="sxs-lookup"><span data-stu-id="326b1-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="326b1-109">[Stáhněte a nainstalujte aplikaci Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)a pokud je to možné, nainstalujte Teams jako správce (klikněte pravým tlačítkem na instalační program Teams a vyberte "Spustit jako správce", pokud je k dispozici).</span><span class="sxs-lookup"><span data-stu-id="326b1-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="326b1-110">Pokud váš klient Teams pořád dochází k chybě, můžete problém reprodukovat?</span><span class="sxs-lookup"><span data-stu-id="326b1-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="326b1-111">Pokud ano:</span><span class="sxs-lookup"><span data-stu-id="326b1-111">If so:</span></span>

1. <span data-ttu-id="326b1-112">K zachycení kroků použijte Záznam kroků.</span><span class="sxs-lookup"><span data-stu-id="326b1-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="326b1-113">Zavřete všechny nepotřebné nebo důvěrné aplikace.</span><span class="sxs-lookup"><span data-stu-id="326b1-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="326b1-114">Spusťte záznam kroků a reprodukovat problém při přihlášení pomocí ovlivněného uživatelského účtu.</span><span class="sxs-lookup"><span data-stu-id="326b1-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="326b1-115">[Shromážděte protokoly týmů, které zaznamenávají zaznamenané kroky reprocesu](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="326b1-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="326b1-116">**Poznámka:** Ujistěte se, že zaznamenáte přihlašovací adresu ovlivněné uživatele.</span><span class="sxs-lookup"><span data-stu-id="326b1-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="326b1-117">Shromážděte informace o kontejneru stavu a/nebo chybovém kontejneru (Windows).</span><span class="sxs-lookup"><span data-stu-id="326b1-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="326b1-118">Spusťte Windows PowerShell na počítači, kde k chybě dochází, a spusťte následující příkazy:</span><span class="sxs-lookup"><span data-stu-id="326b1-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="326b1-119">Připojte soubor k případu podpory.</span><span class="sxs-lookup"><span data-stu-id="326b1-119">Attach the file to your support case.</span></span>
