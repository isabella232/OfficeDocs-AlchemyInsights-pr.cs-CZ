---
title: 1065 neEOP odchozí IP adresy rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806788"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="40015-102">NeEOPování odchozích rozsahů IP adres</span><span class="sxs-lookup"><span data-stu-id="40015-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="40015-103">Zjistili jsme potenciální problém ve vaší organizaci, který (Pokud není opraven 26th) 2018, může přerušit tok pošty do místních nebo externích cílů.</span><span class="sxs-lookup"><span data-stu-id="40015-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="40015-104">Pokud chcete správu rozsahu IP adres zjednodušit, slučujeme rozsahy IP adres ochrany Exchange Online (EOP), které se používají k posílání a přijímání e-mailů mimo Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="40015-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="40015-105">Naše analýza naznačuje, že jeden nebo více externích zdrojů nebo cílů, které jste nakonfigurovali ve spojnicích toku pošty, nepřijímá připojení ze [zde](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)uvedených rozsahů IP adres.</span><span class="sxs-lookup"><span data-stu-id="40015-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="40015-106">Zajistěte, aby tyto zdroje a cíle přijímaly připojení ke všem [publikovaným EOP adresám](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)a 26th.</span><span class="sxs-lookup"><span data-stu-id="40015-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="40015-107">Další informace o této změně naleznete v centru zpráv příspěvky [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)nebo [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="40015-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="40015-108">**Poznámka**: Pokud jste v rámci aktualizací koncového bodu používali funkci publikování na adresy IP, XML a RSS, měli byste také migrovat do nových webových služeb pro automatizaci těchto typů aktualizací.</span><span class="sxs-lookup"><span data-stu-id="40015-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="40015-109">Další informace najdete v tématech [kategorie koncového bodu microsoft 365 a webová služba IP adresa a URL microsoft 365](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="40015-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
