---
title: 'Skener AIP: instalace a konfigurace'
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
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821656"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="efea5-102">Skener AIP: instalace a konfigurace</span><span class="sxs-lookup"><span data-stu-id="efea5-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="efea5-103">**Pokud chcete nainstalovat skener AIP, postupujte podle doporučených pokynů**:</span><span class="sxs-lookup"><span data-stu-id="efea5-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="efea5-104">Pokud upgradujete a neinstalujete čistou instalaci, ujistěte se prosím, že jste se řiďte pokyny pro upgrade skeneru [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) a jednotného klienta pro označování, podívejte se na upgrade skeneru Azure [Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="efea5-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="efea5-105">Ověřte, že splňujete všechny [požadavky na nastavení brány Firewall](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)a síťové infrastruktury .</span><span class="sxs-lookup"><span data-stu-id="efea5-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="efea5-106">Ujistěte [se, že jsou zásady nastavené](https://docs.microsoft.com/azure/information-protection/configure-policy) na automatické popisky nebo mají v zásadách výchozí popisek.</span><span class="sxs-lookup"><span data-stu-id="efea5-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="efea5-107">Ujistěte se, že je příslušný typ souboru nakonfigurovaný pro popisek/ochranu, jak je popsáno v článku Typy souborů [podporované klientem Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="efea5-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="efea5-108">Pokud chcete změnit výchozí chování, postupujte podle těchto pokynů: [Změna výchozí úrovně](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)ochrany souborů .</span><span class="sxs-lookup"><span data-stu-id="efea5-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="efea5-109">Ověřte, jestli má uživatelský účet nakonfigurovaný ke spuštění služby skeneru oprávnění pro přístup ke všem nakonfigurované úložišti.</span><span class="sxs-lookup"><span data-stu-id="efea5-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="efea5-110">Pokud máte pořád problémy, vyexportujte protokoly skeneru a přidejte je do lístku podpory.</span><span class="sxs-lookup"><span data-stu-id="efea5-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="efea5-111">**Export protokolů skeneru Ochrany informací v Azure**</span><span class="sxs-lookup"><span data-stu-id="efea5-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="efea5-112">Přejděte do složky %localappdata%\Microsoft\MSIP v kontextu uživatele, ve které běží služba skeneru.</span><span class="sxs-lookup"><span data-stu-id="efea5-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="efea5-113">Zazipujte veškerý obsah ve složce MSIP.</span><span class="sxs-lookup"><span data-stu-id="efea5-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="efea5-114">Protokoly uložte do volby umístění a připojte je k žádosti o službu.</span><span class="sxs-lookup"><span data-stu-id="efea5-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="efea5-115">Můžete taky použít [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="efea5-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="efea5-116">**Další informace najdete v tématu**:</span><span class="sxs-lookup"><span data-stu-id="efea5-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="efea5-117">Nasazení skeneru Azure Information Protection k automatické klasifikaci a ochraně souborů</span><span class="sxs-lookup"><span data-stu-id="efea5-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="efea5-118">Zadání a použití parametru Token pro nastavení AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="efea5-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="efea5-119">Spuštění cyklu zjišťování a zobrazení sestav skeneru</span><span class="sxs-lookup"><span data-stu-id="efea5-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="efea5-120">Kontrola dokumentace k Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="efea5-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="efea5-121">Požadavky na Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="efea5-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="efea5-122">Stažení klienta Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="efea5-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
