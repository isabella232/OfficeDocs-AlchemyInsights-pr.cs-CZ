---
title: Identifikace externího předávání e-mailů u poštovních schránek v protokolech auditování
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696290"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="1d4cd-102">Určení, kdy je u poštovních schránek nakonfigurovaný externí e-mail</span><span class="sxs-lookup"><span data-stu-id="1d4cd-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="1d4cd-103">Když uživatel Microsoft 365 nakonfiguruje externí předávání e-mailů v poštovní schránce, bude auditována jako součást rutiny **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="1d4cd-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="1d4cd-104">Aktivitu můžete zobrazit pomocí vyhledávání v protokolu auditování & centru dodržování předpisů.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="1d4cd-105">Přihlaste se do [centra zabezpečení Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="1d4cd-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="1d4cd-106">Přejděte na stránku **Search**pro  >  **vyhledávání protokolu auditování** .</span><span class="sxs-lookup"><span data-stu-id="1d4cd-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="1d4cd-107">V polích **Datum zahájení** a **Datum ukončení** vyberte rozsah dat.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="1d4cd-108">Nemusíte zadávat uživatelské jméno.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-108">You don't need to specify a username.</span></span> <span data-ttu-id="1d4cd-109">Ověřte, jestli je pole **aktivity** nastaveno tak, aby **zobrazovalo výsledky pro všechny aktivity**.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="1d4cd-110">Klikněte na **Hledat**.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-110">Click **Search**.</span></span>

<span data-ttu-id="1d4cd-111">Ve výsledcích klikněte v poli Filtr aktivity na filtrovat **výsledky** a typ **Nastavení – poštovní schránka** .</span><span class="sxs-lookup"><span data-stu-id="1d4cd-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="1d4cd-112">Ve výsledcích vyberte záznam auditu.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-112">Select an audit record in the results.</span></span> <span data-ttu-id="1d4cd-113">V rozevíracím seznamu **podrobností** klikněte na **Další informace**.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="1d4cd-114">Pokud chcete zjistit, jestli aktivita souvisí s přesměrováním e-mailu, podívejte se na podrobnosti o jednotlivých záznamech auditu.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="1d4cd-115">**ObjectID**: hodnota aliasu poštovní schránky, která byla změněna.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="1d4cd-116">**Parametry**: _ForwardingSmtpAddress_ označuje cílovou e-mailovou adresu.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="1d4cd-117">**UserID**: uživatel, který nakonfigurovali přesměrování e-mailu na poštovní schránku v poli **objectID**</span><span class="sxs-lookup"><span data-stu-id="1d4cd-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="1d4cd-118">Další informace najdete v tématu [určení, kdo nastavil přeposlání e-mailů pro poštovní schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="1d4cd-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
