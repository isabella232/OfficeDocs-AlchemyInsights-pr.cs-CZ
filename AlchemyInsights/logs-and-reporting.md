---
title: Protokoly a vytváření sestav
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035860"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="df00e-102">Protokoly a vytváření sestav</span><span class="sxs-lookup"><span data-stu-id="df00e-102">Logs and Reporting</span></span>

<span data-ttu-id="df00e-103">[Odpovědi na časté otázky k](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) sestavám Azure Active Directory (Azure Active Directory) ve službě Azure Active Directory (Azure AD) najdete v častých otázkách.</span><span class="sxs-lookup"><span data-stu-id="df00e-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="df00e-104">Další informace najdete v [sestavách Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="df00e-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="df00e-105">**Řešení problémů s auditem**</span><span class="sxs-lookup"><span data-stu-id="df00e-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="df00e-106">Pokud máte problémy se sledováním některých aktivit auditování a chybějící aktivita je v tomto [seznamu,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)zapište lístek podpory.</span><span class="sxs-lookup"><span data-stu-id="df00e-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="df00e-107">Pokud máte problémy se zobrazením protokolů auditování ve vašem tenantovi, zapište lístek podpory.</span><span class="sxs-lookup"><span data-stu-id="df00e-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="df00e-108">Pokud se vaše aktivity auditování na portálu Azure [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) Portal nezobrazují okamžitě, podívejte se na informace o latenci a za soubor lístku podpory, pokud zpoždění překročí zdokumentované latenci.</span><span class="sxs-lookup"><span data-stu-id="df00e-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="df00e-109">Uchovávání záznamů o aktivitách služby Azure AD</span><span class="sxs-lookup"><span data-stu-id="df00e-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="df00e-110">Pokud nevidíte všechny auditování pro vybraný rozsah dat, můžete si z portálu Azure Portal stáhnout až 250 řádků (seřazené podle nejnovějších).</span><span class="sxs-lookup"><span data-stu-id="df00e-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="df00e-111">Další informace najdete v článku [o stažení aktivit auditování.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="df00e-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="df00e-112">**Poradce při potížích s přihlášením**</span><span class="sxs-lookup"><span data-stu-id="df00e-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="df00e-113">Data za posledních 30 dní uvidíte jenom v případě, že máte pro klienta licenci Azure AD Premium (P1 nebo P2).</span><span class="sxs-lookup"><span data-stu-id="df00e-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="df00e-114">Přihlášení jsou dostupné jenom pro tenanty Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="df00e-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="df00e-115">Není k dispozici pro bezplatné nebo základní licencované tenanty.</span><span class="sxs-lookup"><span data-stu-id="df00e-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="df00e-116">Pokud má váš tenant licenci Premium P1 a nevidíte přihlášení, podívejte [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) se na informace o latenci a za soubor lístku podpory, pokud zpoždění přesáhne zdokumentované latenci.</span><span class="sxs-lookup"><span data-stu-id="df00e-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="df00e-117">Pokud nevidíte všechny přihlášení k rozsahu dat, který jste vybrali, můžete si z portálu Azure Portal stáhnout až 250 řádků (řazené podle nejnovějších).</span><span class="sxs-lookup"><span data-stu-id="df00e-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="df00e-118">Další informace najdete v článku [o stažení aktivit přihlašování.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="df00e-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="df00e-119">**Řešení potíží se zprávami zabezpečení (uživatelé s příznakem na riziko, riziko přihlášení)**</span><span class="sxs-lookup"><span data-stu-id="df00e-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="df00e-120">Uživatelé označení pro sestavu zabezpečení rizik</span><span class="sxs-lookup"><span data-stu-id="df00e-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="df00e-121">Sestava rizikoových přihlášení na portálu Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="df00e-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="df00e-122">Riskové události Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="df00e-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
