---
title: Identifikace událostí odstranění zpráv v protokolech auditování
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696506"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="23635-102">Protokoly auditování odstraněných e-mailových zpráv</span><span class="sxs-lookup"><span data-stu-id="23635-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="23635-103">Od ledna 2019 společnost Microsoft ve výchozím nastavení zapíná protokolování auditu poštovní schránky.</span><span class="sxs-lookup"><span data-stu-id="23635-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="23635-104">Pokud chcete v opačném případě zkontrolovat odstranění událostí pro konkrétního uživatele, musíte ručně povolit akce odstranění pro auditování.</span><span class="sxs-lookup"><span data-stu-id="23635-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="23635-105">Pokud je protokolování auditu poštovní schránky pro vaši organizaci nebo pro určitého uživatele povolené, postupujte podle následujících kroků.</span><span class="sxs-lookup"><span data-stu-id="23635-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="23635-106">Přihlášení do [centra dodržování předpisů Microsoft 365 Security &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="23635-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="23635-107">Klikněte na **Hledat a vyšetřování** a vyberte **Hledat v protokolu auditování**.</span><span class="sxs-lookup"><span data-stu-id="23635-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="23635-108">V polích **Datum zahájení** a **Datum ukončení** vyberte rozsah dat.</span><span class="sxs-lookup"><span data-stu-id="23635-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="23635-109">Zadejte uživatelské jméno, které chcete prozkoumat (uživatel, který položky odstranil).</span><span class="sxs-lookup"><span data-stu-id="23635-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="23635-110">V poli **aktivity** vyberte **odstraněné zprávy ze složky Odstraněná pošta** a **přesunuté zprávy do složky Odstraněná pošta**.</span><span class="sxs-lookup"><span data-stu-id="23635-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="23635-111">Klikněte na **Hledat**.</span><span class="sxs-lookup"><span data-stu-id="23635-111">Click **Search**.</span></span>

<span data-ttu-id="23635-112">Ve výsledcích vyberte záznam auditu.</span><span class="sxs-lookup"><span data-stu-id="23635-112">In the results, select an audit record.</span></span> <span data-ttu-id="23635-113">V rozevíracím seznamu podrobností klikněte na **Další informace**.</span><span class="sxs-lookup"><span data-stu-id="23635-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="23635-114">Další informace o odstraněné položce (například předmět a umístění položky po jejím odstranění) se zobrazí v poli **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="23635-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="23635-115">Vlastnost **ClientInfoString** se zobrazí, pokud v Outlooku, Outlooku na webu (dřív se říká Outlook Web App) nebo jiném zařízení.</span><span class="sxs-lookup"><span data-stu-id="23635-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="23635-116">Další informace najdete v tématu [určení, kdo nastavil přeposlání e-mailů pro poštovní schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="23635-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="23635-117">**Poznámka**: odstraněné položky nemůžete načíst pomocí funkce protokol auditování.</span><span class="sxs-lookup"><span data-stu-id="23635-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="23635-118">Pokud chcete v Outlooku na webu načíst odstraněné zprávy, přečtěte si článek [obnovení odstraněných položek v Outlook Web Appu](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="23635-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
