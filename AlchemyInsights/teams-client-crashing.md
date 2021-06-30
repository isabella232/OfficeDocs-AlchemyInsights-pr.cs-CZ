---
title: Teams klienta dojde k chybě
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187714"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="8ae20-102">Teams klienta dojde k chybě</span><span class="sxs-lookup"><span data-stu-id="8ae20-102">Teams client crashing</span></span>

<span data-ttu-id="8ae20-103">Pokud v klientovi Teams dochází k chybám, vyzkoušejte následující postup:</span><span class="sxs-lookup"><span data-stu-id="8ae20-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="8ae20-104">Pokud používáte desktopovou aplikaci Teams, [zkontrolujte, jestli je tato aplikace kompletně aktualizovaná](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="8ae20-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="8ae20-105">Ujistěte se, [že jsou Microsoft 365 adresy URL a rozsahy adres](/microsoftteams/connectivity-issues) přístupné.</span><span class="sxs-lookup"><span data-stu-id="8ae20-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="8ae20-106">Přihlaste se pomocí účtu správce tenanta a zkontrolujte řídicí panel [stavu služby,](/office365/enterprise/view-service-health) abyste ověřili, že neexistuje žádný výpadk nebo degradace služby.</span><span class="sxs-lookup"><span data-stu-id="8ae20-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="8ae20-107">Odinstalace a přeinstalace Teams aplikace</span><span class="sxs-lookup"><span data-stu-id="8ae20-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="8ae20-108">Přejděte do složky %appdata%\Microsoft\Teams\ na počítači a odstraňte všechny soubory v tomto adresáři.</span><span class="sxs-lookup"><span data-stu-id="8ae20-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="8ae20-109">[Stáhněte a nainstalujte aplikaci Teams a](https://www.microsoft.com/microsoft-teams/download-app)pokud je to možné, nainstalujte Teams jako správce (klikněte  pravým tlačítkem na instalační program Teams a vyberte Spustit jako správce, pokud je k dispozici).</span><span class="sxs-lookup"><span data-stu-id="8ae20-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="8ae20-110">Pokud váš Teams klient stále dochází k chybě, zkuste problém reprodukovat.</span><span class="sxs-lookup"><span data-stu-id="8ae20-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="8ae20-111">Pokud můžete:</span><span class="sxs-lookup"><span data-stu-id="8ae20-111">If you can:</span></span>

1. <span data-ttu-id="8ae20-112">K zachycení kroků použijte Záznam kroků.</span><span class="sxs-lookup"><span data-stu-id="8ae20-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="8ae20-113">Zavřete všechny nepotřebné nebo důvěrné aplikace.</span><span class="sxs-lookup"><span data-stu-id="8ae20-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="8ae20-114">Spusťte záznam kroků a reprodukovat problém při přihlášení pomocí ovlivněného uživatelského účtu.</span><span class="sxs-lookup"><span data-stu-id="8ae20-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="8ae20-115">[Shromážděte protokoly týmů, které zaznamenávají zaznamenané kroky reprocesu](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="8ae20-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="8ae20-116">**Poznámka:** Ujistěte se, že zaznamenáte přihlašovací adresu ovlivněné uživatele.</span><span class="sxs-lookup"><span data-stu-id="8ae20-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="8ae20-117">Shromážděte informace o kontejneru stavu a/nebo chybovém kontejneru (Windows).</span><span class="sxs-lookup"><span data-stu-id="8ae20-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="8ae20-118">Spusťte Windows powershellu na počítači, kde k chybě dochází, a spusťte následující příkazy (po každém příkazu stiskněte Enter):</span><span class="sxs-lookup"><span data-stu-id="8ae20-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="8ae20-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="8ae20-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="8ae20-120">Po vygenerování textového souboru, který se zobrazí na obrazovce, uložte soubor a připojte ho k žádosti o službu.</span><span class="sxs-lookup"><span data-stu-id="8ae20-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
