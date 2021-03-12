---
title: Automatické přesunutí e-mailových zpráv do archivační poštovní schránky
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744548"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="1fb67-102">Automatické přesunutí e-mailových zpráv do archivační poštovní schránky</span><span class="sxs-lookup"><span data-stu-id="1fb67-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="1fb67-103">Tady je postup, jak nastavit zásadu pro automatické přesunutí starého e-mailu uživatele do archivační poštovní schránky:</span><span class="sxs-lookup"><span data-stu-id="1fb67-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="1fb67-104">Přejděte na [**Archiv & správy**](https://go.microsoft.com/fwlink/p/?linkid=2077143)dat dodržování předpisů a ověřte, jestli je pro uživatele povolená  >    >   archivační poštovní schránka.</span><span class="sxs-lookup"><span data-stu-id="1fb67-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="1fb67-105">Pokud tomu tak není,  klikněte v poli upozornění na **Povolit** a pak na Ano.</span><span class="sxs-lookup"><span data-stu-id="1fb67-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="1fb67-106">Přejděte do [**Centra pro správu Exchange > dodržování předpisů > značky uchovávání informací**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="1fb67-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="1fb67-107">Zvolte ikonu + a pak zvolte **automaticky použít pro celou poštovní schránku**.</span><span class="sxs-lookup"><span data-stu-id="1fb67-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="1fb67-108">Přiřaďte název značce uchovávání informací a zvolte **Přesunout do archivu**.</span><span class="sxs-lookup"><span data-stu-id="1fb67-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="1fb67-109">Pro dobu uchovávání zadejte dobu, kterou chcete, například 90 dnů.</span><span class="sxs-lookup"><span data-stu-id="1fb67-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="1fb67-110">Klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="1fb67-110">Click **Save**.</span></span>
5. <span data-ttu-id="1fb67-111">Teď vytvořte zásadu uchovávání informací: zvolte zásady **uchovávání** informací , zvolte ikonu a přidejte novou zásadu.</span><span class="sxs-lookup"><span data-stu-id="1fb67-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="1fb67-112">Přiřaďte k zásadám uchovávání informací název, potom kliknutím a posouváním vyhledejte a přidejte značku uchovávání informací, kterou jste právě vytvořili.</span><span class="sxs-lookup"><span data-stu-id="1fb67-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="1fb67-113">Klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="1fb67-113">Click **Save**.</span></span>
7. <span data-ttu-id="1fb67-114">Nakonec použijte zásady uchovávání informací pro poštovní schránku uživatele: pořád v Centru pro správu Exchange přejděte na **poštovní schránky**  >  **příjemců**.</span><span class="sxs-lookup"><span data-stu-id="1fb67-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="1fb67-115">Vyberte všechny uživatele, u kterého chcete zásadu použít, a pak zvolte **Upravit** (ikona tužky).</span><span class="sxs-lookup"><span data-stu-id="1fb67-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="1fb67-116">V dialogovém okně klikněte na funkce **poštovní schránky**.</span><span class="sxs-lookup"><span data-stu-id="1fb67-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="1fb67-117">V **části Zásady uchovávání** informací použijte zásadu, kterou jste právě vytvořili, > **Uložit.**</span><span class="sxs-lookup"><span data-stu-id="1fb67-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="1fb67-118">Pokyny k použití zásad pro všechny uživatele najdete v článku Použití zásad [uchovávání informací u poštovních schránek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="1fb67-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
