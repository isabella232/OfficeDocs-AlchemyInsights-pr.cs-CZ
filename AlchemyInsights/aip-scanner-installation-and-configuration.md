---
title: 'AIP Scanner: instalace a konfigurace'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686635"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="7e780-102">AIP Scanner: instalace a konfigurace</span><span class="sxs-lookup"><span data-stu-id="7e780-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="7e780-103">Pokud **chcete nainstalovat skener AIP, postupujte podle doporučených pokynů**:</span><span class="sxs-lookup"><span data-stu-id="7e780-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="7e780-104">Pokud inovujete a neprovedete čistou instalaci, [Ujistěte se,](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)že jste postupovali podle pokynů pro [upgrade skeneru ochrany informací Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) a pro jednotné klienty s popisem.</span><span class="sxs-lookup"><span data-stu-id="7e780-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="7e780-105">Ověřte, že dodržujete všechny [požadavky brány firewall a nastavení síťové infrastruktury](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="7e780-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="7e780-106">Ujistěte se, že [jsou vaše zásady nastavené](https://docs.microsoft.com/azure/information-protection/configure-policy) na automatický popis nebo mají v zásadě výchozí popisek.</span><span class="sxs-lookup"><span data-stu-id="7e780-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="7e780-107">Ujistěte se, že příslušný typ souboru je nakonfigurovaný pro popisek nebo ochranu, jak je popsáno v [typech souborů podporovaných klientem ochrany informací Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="7e780-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="7e780-108">Pokud chcete změnit výchozí chování, postupujte podle těchto pokynů: [Změna výchozí úrovně ochrany souborů](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="7e780-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="7e780-109">Ověřte, že uživatelský účet nakonfigurovaný pro spuštění služby skeneru má oprávnění k přístupu ke všem nakonfigurovaným úložištím.</span><span class="sxs-lookup"><span data-stu-id="7e780-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="7e780-110">Pokud pořád dochází k problémům, exportujte protokoly skeneru a přidejte je do lístku podpory.</span><span class="sxs-lookup"><span data-stu-id="7e780-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="7e780-111">**Export protokolů skeneru služby Azure Information Protection**</span><span class="sxs-lookup"><span data-stu-id="7e780-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="7e780-112">V kontextu uživatele, který spouští službu skeneru, přejděte na%localappdata%\Microsoft\MSIP.</span><span class="sxs-lookup"><span data-stu-id="7e780-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="7e780-113">Zip All (obsah) ve složce MSIP</span><span class="sxs-lookup"><span data-stu-id="7e780-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="7e780-114">Protokoly uložte na svůj výběr a připojte je k žádosti o služby.</span><span class="sxs-lookup"><span data-stu-id="7e780-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="7e780-115">Můžete taky použít funkci [exportovat – AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="7e780-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="7e780-116">**Další informace najdete v těchto tématech**:</span><span class="sxs-lookup"><span data-stu-id="7e780-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="7e780-117">Nasazení skeneru ochrany informací Azure pro automatické klasifikaci a ochranu souborů</span><span class="sxs-lookup"><span data-stu-id="7e780-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="7e780-118">Určení a použití parametru tokenu pro set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="7e780-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="7e780-119">Spuštění cyklu zjišťování a zobrazení sestav pro skener</span><span class="sxs-lookup"><span data-stu-id="7e780-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="7e780-120">Přečtěte si dokumentaci k Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7e780-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="7e780-121">Požadavky na ochranu informací Azure</span><span class="sxs-lookup"><span data-stu-id="7e780-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="7e780-122">Stáhnout klienta ochrany informací v Azure</span><span class="sxs-lookup"><span data-stu-id="7e780-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
