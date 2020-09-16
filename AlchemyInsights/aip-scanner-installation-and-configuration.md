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
# <a name="aip-scanner-installation-and-configuration"></a>AIP Scanner: instalace a konfigurace

Pokud **chcete nainstalovat skener AIP, postupujte podle doporučených pokynů**:

1. Pokud inovujete a neprovedete čistou instalaci, [Ujistěte se,](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)že jste postupovali podle pokynů pro [upgrade skeneru ochrany informací Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) a pro jednotné klienty s popisem.
2. Ověřte, že dodržujete všechny [požadavky brány firewall a nastavení síťové infrastruktury](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Ujistěte se, že [jsou vaše zásady nastavené](https://docs.microsoft.com/azure/information-protection/configure-policy) na automatický popis nebo mají v zásadě výchozí popisek.
4. Ujistěte se, že příslušný typ souboru je nakonfigurovaný pro popisek nebo ochranu, jak je popsáno v [typech souborů podporovaných klientem ochrany informací Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Pokud chcete změnit výchozí chování, postupujte podle těchto pokynů: [Změna výchozí úrovně ochrany souborů](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Ověřte, že uživatelský účet nakonfigurovaný pro spuštění služby skeneru má oprávnění k přístupu ke všem nakonfigurovaným úložištím.
6. Pokud pořád dochází k problémům, exportujte protokoly skeneru a přidejte je do lístku podpory.

**Export protokolů skeneru služby Azure Information Protection**

1. V kontextu uživatele, který spouští službu skeneru, přejděte na%localappdata%\Microsoft\MSIP.
2. Zip All (obsah) ve složce MSIP
3. Protokoly uložte na svůj výběr a připojte je k žádosti o služby.
4. Můžete taky použít funkci [exportovat – AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Další informace najdete v těchto tématech**:
- [Nasazení skeneru ochrany informací Azure pro automatické klasifikaci a ochranu souborů](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Určení a použití parametru tokenu pro set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Spuštění cyklu zjišťování a zobrazení sestav pro skener](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Přečtěte si dokumentaci k Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Požadavky na ochranu informací Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Stáhnout klienta ochrany informací v Azure](https://www.microsoft.com/download/details.aspx?id=53018)
