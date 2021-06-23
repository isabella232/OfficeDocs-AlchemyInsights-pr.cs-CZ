---
title: Povolení ověřování SMTP a odstraňování potíží
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077644"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="6a583-102">Povolení ověřování SMTP a odstraňování potíží</span><span class="sxs-lookup"><span data-stu-id="6a583-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="6a583-103">Pokud chcete povolit ověřování SMTP pro poštovní schránku nebo se zobrazí chyba "Klient není ověřen", "Ověřování neúspěšné" nebo "SmtpClientAuthentication" s kódem 5.7.57 nebo 5.7.3 nebo 5.7.139 při pokusu o přenos e-mailů ověřením zařízení nebo aplikace s Microsoft 365, proveďte tyto tři akce k vyřešení problému:</span><span class="sxs-lookup"><span data-stu-id="6a583-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="6a583-104">Výchozí nastavení [zabezpečení Azure můžete zakázat](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) tak, že **povolíte výchozí nastavení zabezpečení** na **Ne**.</span><span class="sxs-lookup"><span data-stu-id="6a583-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="6a583-105">a.</span><span class="sxs-lookup"><span data-stu-id="6a583-105">a.</span></span> <span data-ttu-id="6a583-106">Přihlaste se k webu Azure Portal jako správce zabezpečení, správce podmíněného přístupu nebo globální správce.</span><span class="sxs-lookup"><span data-stu-id="6a583-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="6a583-107">b.</span><span class="sxs-lookup"><span data-stu-id="6a583-107">b.</span></span> <span data-ttu-id="6a583-108">Přejděte na Azure Active Directory > **vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="6a583-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="6a583-109">c.</span><span class="sxs-lookup"><span data-stu-id="6a583-109">c.</span></span> <span data-ttu-id="6a583-110">Vyberte **Spravovat výchozí nastavení zabezpečení**.</span><span class="sxs-lookup"><span data-stu-id="6a583-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="6a583-111">d.</span><span class="sxs-lookup"><span data-stu-id="6a583-111">d.</span></span> <span data-ttu-id="6a583-112">Nastavte **povolit výchozí nastavení zabezpečení na** **Ne**.</span><span class="sxs-lookup"><span data-stu-id="6a583-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="6a583-113">e.</span><span class="sxs-lookup"><span data-stu-id="6a583-113">e.</span></span> <span data-ttu-id="6a583-114">Vyberte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="6a583-114">Select **Save**.</span></span>

2. <span data-ttu-id="6a583-115">[Povolte odeslání smtp klienta](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) u licencované poštovní schránky.</span><span class="sxs-lookup"><span data-stu-id="6a583-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="6a583-116">a.</span><span class="sxs-lookup"><span data-stu-id="6a583-116">a.</span></span> <span data-ttu-id="6a583-117">V Centrum pro správu Microsoftu 365 přejděte na **Aktivní uživatelé** a vyberte uživatele.</span><span class="sxs-lookup"><span data-stu-id="6a583-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="6a583-118">b.</span><span class="sxs-lookup"><span data-stu-id="6a583-118">b.</span></span> <span data-ttu-id="6a583-119">Přejděte na kartu Pošta a v části **E-mailové aplikace** vyberte **Spravovat e-mailové aplikace**.</span><span class="sxs-lookup"><span data-stu-id="6a583-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="6a583-120">d.</span><span class="sxs-lookup"><span data-stu-id="6a583-120">d.</span></span> <span data-ttu-id="6a583-121">Ujistěte **se, že je zaškrtnuté** políčko Ověřený protokol SMTP (povoleno).</span><span class="sxs-lookup"><span data-stu-id="6a583-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="6a583-122">e.</span><span class="sxs-lookup"><span data-stu-id="6a583-122">e.</span></span> <span data-ttu-id="6a583-123">Vyberte **Uložit změny**.</span><span class="sxs-lookup"><span data-stu-id="6a583-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="6a583-124">[V licencované poštovní schránce zakažte](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) vícefaktorové ověřování (MFA).</span><span class="sxs-lookup"><span data-stu-id="6a583-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="6a583-125">a.</span><span class="sxs-lookup"><span data-stu-id="6a583-125">a.</span></span> <span data-ttu-id="6a583-126">Přejděte na Centrum pro správu Microsoftu 365 a v levé navigační nabídce vyberte **Uživatelé**  >  **aktivní uživatelé**.</span><span class="sxs-lookup"><span data-stu-id="6a583-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="6a583-127">b.</span><span class="sxs-lookup"><span data-stu-id="6a583-127">b.</span></span> <span data-ttu-id="6a583-128">Vyberte **Vícefaktorové ověřování**.</span><span class="sxs-lookup"><span data-stu-id="6a583-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="6a583-129">c.</span><span class="sxs-lookup"><span data-stu-id="6a583-129">c.</span></span> <span data-ttu-id="6a583-130">Vyberte uživatele a **zakažte vícefaktorové ověřování**.</span><span class="sxs-lookup"><span data-stu-id="6a583-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
