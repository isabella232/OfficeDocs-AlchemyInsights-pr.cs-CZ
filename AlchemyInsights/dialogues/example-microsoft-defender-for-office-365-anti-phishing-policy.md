---
title: Příklad anti-phishingové zásady Microsoft Defenderu pro Office 365
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
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693240"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="1810d-102">Příklad anti-phishingové zásady Microsoft Defenderu pro Office 365</span><span class="sxs-lookup"><span data-stu-id="1810d-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="1810d-103">Toto nastavení umožňuje zásady s názvem Doména a *generálního ředitele.*</span><span class="sxs-lookup"><span data-stu-id="1810d-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="1810d-104">Tato zásada poskytuje ochranu před zosobněním uživatele i domény a pak je použije pro všechny e-maily přijaté uživateli v doméně.</span><span class="sxs-lookup"><span data-stu-id="1810d-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="1810d-105">Nejdřív přidejte následující informace k vytvoření zásady:</span><span class="sxs-lookup"><span data-stu-id="1810d-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="1810d-106">**Název:** Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span><span class="sxs-lookup"><span data-stu-id="1810d-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="1810d-107">**Platí pro:** Vyberte **doménu příjemce.**</span><span class="sxs-lookup"><span data-stu-id="1810d-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="1810d-108">V **části Libovolná z těchto** možností vyberte **Možnost** a pak vyberte doménu.</span><span class="sxs-lookup"><span data-stu-id="1810d-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="1810d-109">Vyberte **+ Přidat.**</span><span class="sxs-lookup"><span data-stu-id="1810d-109">Select **+ Add**.</span></span> <span data-ttu-id="1810d-110">Zaškrtněte políčko vedle názvu domény v seznamu (například contoso.com *)* a pak vyberte **Přidat.**</span><span class="sxs-lookup"><span data-stu-id="1810d-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="1810d-111">Vyberte **Hotovo.**</span><span class="sxs-lookup"><span data-stu-id="1810d-111">Select **Done**.</span></span>
- <span data-ttu-id="1810d-112">Po vytvoření zásady můžete zásadu vyladit pomocí následujících možností:</span><span class="sxs-lookup"><span data-stu-id="1810d-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="1810d-113">**Ochrana přidáním uživatelů:** V tomto příkladu přidejte minimálně e-mailovou adresu generálního ředitele.</span><span class="sxs-lookup"><span data-stu-id="1810d-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="1810d-114">**Přidání domén pro ochranu:** Přidejte doménu organizace, která obsahuje kancelář generálního ředitele.</span><span class="sxs-lookup"><span data-stu-id="1810d-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="1810d-115">**Zvolte akce:** **Pokud** e-mail posílá uživatel zosobněného uživatele, vyberte Přesměrovat zprávu na jinou e-mailovou adresu a potom zadejte e-mailovou adresu správce zabezpečení (například *securityadmin@contoso.com).*</span><span class="sxs-lookup"><span data-stu-id="1810d-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="1810d-116">Pokud **e-mail posíláte zosobněná doména,** vyberte **Přesunout zprávu do karantény.**</span><span class="sxs-lookup"><span data-stu-id="1810d-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="1810d-117">**Inteligentní poštovní** schránka: Ve výchozím nastavení je tato možnost vybraná, když vytváříte novou anti-phishingovou zásadu.</span><span class="sxs-lookup"><span data-stu-id="1810d-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="1810d-118">Nejlepších výsledků **dosáhnete,** když toto nastavení necháte zas.</span><span class="sxs-lookup"><span data-stu-id="1810d-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="1810d-119">**Přidání důvěryhodných odesílatelů** a domén: V tomto příkladu nedefinujte žádné přepsání.</span><span class="sxs-lookup"><span data-stu-id="1810d-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="1810d-120">Až nastavení prošetříte, vyberte Podle potřeby Vytvořit tuto zásadu nebo **Uložit.** </span><span class="sxs-lookup"><span data-stu-id="1810d-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="1810d-121">Další informace najdete v [anti-phishingových zásadách v Microsoftu 365.](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="1810d-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
