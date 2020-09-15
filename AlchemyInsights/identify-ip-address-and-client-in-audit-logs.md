---
title: Identifikace IP adresy a klienta v protokolech auditování
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668303"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="bc901-102">Identifikace IP adresy a klienta v protokolech auditování</span><span class="sxs-lookup"><span data-stu-id="bc901-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="bc901-103">V protokolech auditování se zobrazuje IP adresa, která odpovídá aktivitě od uživatele Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bc901-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="bc901-104">Informace o klientovi jsou protokolovány také.</span><span class="sxs-lookup"><span data-stu-id="bc901-104">The client information is also logged.</span></span> <span data-ttu-id="bc901-105">Tady je postup, jak tyto informace zjistit.</span><span class="sxs-lookup"><span data-stu-id="bc901-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="bc901-106">Přihlaste se do [centra zabezpečení Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="bc901-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="bc901-107">Přejděte na stránku **Search**pro  >  **vyhledávání protokolu auditování** .</span><span class="sxs-lookup"><span data-stu-id="bc901-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="bc901-108">Pokud máte zájem o konkrétní aktivitu, vyberte ji ze seznamu **aktivity** .</span><span class="sxs-lookup"><span data-stu-id="bc901-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="bc901-109">Pokud ne, budou pro vybraného uživatele (výchozí nastavení) vráceny všechny aktivity.</span><span class="sxs-lookup"><span data-stu-id="bc901-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="bc901-110">**Poznámka**: určité aktivity nemusí být dostupné v nabídce **aktivity** . Tyto položky auditu budou vráceny, pokud je vybrána možnost **Zobrazit výsledky pro všechny aktivity** (výchozí nastavení).</span><span class="sxs-lookup"><span data-stu-id="bc901-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="bc901-111">V poli **Uživatelé** zadejte uživatelské jméno, vyberte odpovídající rozsah kalendářních dat a klikněte na **Hledat**.</span><span class="sxs-lookup"><span data-stu-id="bc901-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="bc901-112">Ve výsledcích se zobrazí IP adresa této aktivity v podokně výsledků.</span><span class="sxs-lookup"><span data-stu-id="bc901-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="bc901-113">Pokud chcete zobrazit podrobné informace v informačním panelu **podrobností** (například klient, uživatel, který provedl akci atd.), vyberte záznam auditování.</span><span class="sxs-lookup"><span data-stu-id="bc901-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="bc901-114">Další informace najdete v tématu [Vyhledání IP adresy počítače použitého pro přístup k ohroženému účtu](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="bc901-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
