---
title: Problémy s SharePoint na Windows 7 počítačích
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
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/28/2021
ms.locfileid: "52124922"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="19c30-102">Problémy s SharePoint na Windows 7 počítačích</span><span class="sxs-lookup"><span data-stu-id="19c30-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="19c30-103">Pokud se při práci na SharePoint nebo OneDrive zobrazí chyby na počítačích Windows 7, můžou souviset s vymazáváním TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="19c30-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="19c30-104">Další informace najdete tady:</span><span class="sxs-lookup"><span data-stu-id="19c30-104">For more information, see:</span></span>

- [<span data-ttu-id="19c30-105">Připravuje se na TLS 1.2 v Office 365 a Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="19c30-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="19c30-106">Windows 7 SP1/Windows 8 klienti musí mít povolený tls1.2.</span><span class="sxs-lookup"><span data-stu-id="19c30-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="19c30-107">Další informace najdete v tématu Chyby ověřování, když [klient nemá podporu TLS 1.2.](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="19c30-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="19c30-108">Nainstalujte KB3140245 a vytvořte hodnotu registru.</span><span class="sxs-lookup"><span data-stu-id="19c30-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="19c30-109">Další informace najdete v článku Aktualizace a povolení [tls 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) jako výchozích zabezpečených protokolů ve WinHTTP v Windows</span><span class="sxs-lookup"><span data-stu-id="19c30-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="19c30-110">Windows 7 SP1/Windows 8 musí zajistit instalaci nejnovějších šifrovacích sad TLS.</span><span class="sxs-lookup"><span data-stu-id="19c30-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="19c30-111">Další informace najdete v tématu [Informační zpravodaj zabezpečení společnosti Microsoft 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span><span class="sxs-lookup"><span data-stu-id="19c30-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


