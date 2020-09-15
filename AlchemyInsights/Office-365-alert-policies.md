---
title: 1385-Office-365-Alert-zásady
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 8821a2ee1ae2207de5d1604762badf43808373c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664019"
---
# <a name="alert-policies"></a><span data-ttu-id="72705-102">Zásady upozornění</span><span class="sxs-lookup"><span data-stu-id="72705-102">Alert policies</span></span>

<span data-ttu-id="72705-103">Centrum kompatibility Microsoft 365 Security & nabízí [výchozí zásady pro výstrahy](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) , které aktivují upozornění pro organizace s předplatným Office 365 Enterprise nebo Office 365 pro vládní organizace verze E1/G1, E3/G3 nebo E5/G5.</span><span class="sxs-lookup"><span data-stu-id="72705-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="72705-104">Správci proto můžou obdržet upozornění e-mailem s upozorněním, které poslal Office365Alerts@microsoft.com s řádkem předmětu, jako je třeba upozornění na nízkou závažnost: *název zásad upozornění*.</span><span class="sxs-lookup"><span data-stu-id="72705-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="72705-105">Oznámení se odesílají, když se aktivují výstrahy pro běžné aktivity, jako jsou třeba uživatelé:</span><span class="sxs-lookup"><span data-stu-id="72705-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="72705-106">Vytvořte pravidla doručené pošty, která přesměrují e-mail.</span><span class="sxs-lookup"><span data-stu-id="72705-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="72705-107">Přiřaďte oprávnění k poštovní schránce.</span><span class="sxs-lookup"><span data-stu-id="72705-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="72705-108">Sdílejte nebo odstraňte velký počet souborů v SharePointovém sdílení souborů.</span><span class="sxs-lookup"><span data-stu-id="72705-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="72705-109">Vytváření hledání v eDiscovery a export výsledků hledání</span><span class="sxs-lookup"><span data-stu-id="72705-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="72705-110">Kontrola a činnost výstrahy:</span><span class="sxs-lookup"><span data-stu-id="72705-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="72705-111">Přejděte do [centra dodržování předpisů &](https://protection.office.com) a přihlaste se.</span><span class="sxs-lookup"><span data-stu-id="72705-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="72705-112">Klikněte **na upozornění**  >  **zobrazení**upozornění.</span><span class="sxs-lookup"><span data-stu-id="72705-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="72705-113">Kliknutím na upozornění zobrazte stránku s informacemi o výstraze.</span><span class="sxs-lookup"><span data-stu-id="72705-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="72705-114">S upozorněním můžete udělat nějakou akci, třeba [Odebrat podezřelé pravidlo doručené pošty](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span><span class="sxs-lookup"><span data-stu-id="72705-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="72705-115">Nebo můžete upozornění zavřít pouhým kliknutím na tlačítko **vyřešit** na stránce se zobrazením informační rámeček upozornění.</span><span class="sxs-lookup"><span data-stu-id="72705-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="72705-116">Další informace o konfiguraci a správě zásad výstrah najdete v  [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="72705-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span></span>

<span data-ttu-id="72705-117">**Důležité**upozornění: upozornění e-mailem od Microsoftu vás nikdy nevyzve k provedení následujících akcí:</span><span class="sxs-lookup"><span data-stu-id="72705-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="72705-118">Zadání hesla</span><span class="sxs-lookup"><span data-stu-id="72705-118">Provide a password</span></span>
- <span data-ttu-id="72705-119">Ověření detailů zabezpečení účtu</span><span class="sxs-lookup"><span data-stu-id="72705-119">Verify the security details of your account</span></span>
- <span data-ttu-id="72705-120">Znovu ověřit</span><span class="sxs-lookup"><span data-stu-id="72705-120">Re-authenticate yourself</span></span>

<span data-ttu-id="72705-121">Pokud dostanete e-mailovou zprávu, která se vám líbí, nebyla odeslána společností Microsoft a měla by být považována za nevydanou podvodnou poštu.</span><span class="sxs-lookup"><span data-stu-id="72705-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="72705-122">Pokud se to stane, [ohlaste to Microsoftu](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span><span class="sxs-lookup"><span data-stu-id="72705-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>