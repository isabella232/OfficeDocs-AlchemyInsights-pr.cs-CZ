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
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934250"
---
# <a name="aip-scanner-installation-and-configuration"></a>Skener AIP: instalace a konfigurace

**Pokud chcete nainstalovat skener AIP, postupujte podle doporučených pokynů**:

1. Pokud upgradujete a neinstalujete čistou instalaci, ujistěte se prosím, že jste se řiďte pokyny pro upgrade skeneru [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) a jednotného klienta pro označování, podívejte se na upgrade skeneru Azure [Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Ověřte, že splňujete všechny [požadavky na nastavení brány Firewall](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)a síťové infrastruktury .
3. Ujistěte [se, že jsou zásady nastavené](https://docs.microsoft.com/azure/information-protection/configure-policy) na automatické popisky nebo mají v zásadách výchozí popisek.
4. Ujistěte se, že je příslušný typ souboru nakonfigurovaný pro popisek/ochranu, jak je popsáno v článku Typy souborů [podporované klientem Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Pokud chcete změnit výchozí chování, postupujte podle těchto pokynů: [Změna výchozí úrovně](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)ochrany souborů .
5. Ověřte, jestli má uživatelský účet nakonfigurovaný ke spuštění služby skeneru oprávnění pro přístup ke všem nakonfigurované úložišti.
6. Pokud máte pořád problémy, vyexportujte protokoly skeneru a přidejte je do lístku podpory.

**Export protokolů skeneru Ochrany informací v Azure**

1. Přejděte do složky %localappdata%\Microsoft\MSIP v kontextu uživatele, ve které běží služba skeneru.
2. Zazipujte veškerý obsah ve složce MSIP.
3. Protokoly uložte do volby umístění a připojte je k žádosti o službu.
4. Můžete taky použít [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Další informace najdete v tématu**:
- [Nasazení skeneru Azure Information Protection k automatické klasifikaci a ochraně souborů](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Zadání a použití parametru Token pro nastavení AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Spuštění cyklu zjišťování a zobrazení sestav skeneru](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Kontrola dokumentace k Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Požadavky na Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Stažení klienta Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
