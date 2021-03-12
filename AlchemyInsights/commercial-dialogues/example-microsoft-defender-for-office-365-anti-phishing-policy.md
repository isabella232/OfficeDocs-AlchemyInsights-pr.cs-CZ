---
title: Příklad zásad ochrany proti phishingu v Microsoft Defenderu pro Office 365
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744896"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="82e2b-102">Příklad zásad ochrany proti phishingu v Microsoft Defenderu pro Office 365</span><span class="sxs-lookup"><span data-stu-id="82e2b-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="82e2b-103">Tato nastavení povolte zásadu s názvem Doména a *výkonný ředitel*.</span><span class="sxs-lookup"><span data-stu-id="82e2b-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="82e2b-104">Tato zásada poskytuje ochranu uživatelů i domén před zosobněním a pak platí pro všechny e-maily přijaté uživateli v doméně.</span><span class="sxs-lookup"><span data-stu-id="82e2b-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="82e2b-105">Nejdřív přidejte následující informace k vytvoření zásady:</span><span class="sxs-lookup"><span data-stu-id="82e2b-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="82e2b-106">**Název:** Domain and CEO **Description**(Popis domény a generálního ředitele): Ujistěte se, že se výkonný ředitel a vaše doména nezosobní.</span><span class="sxs-lookup"><span data-stu-id="82e2b-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="82e2b-107">**Platí pro:** Vyberte **Doména příjemce je**.</span><span class="sxs-lookup"><span data-stu-id="82e2b-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="82e2b-108">V **části Kterýkoli z těchto** možností vyberte **Zvolit** a pak vyberte doménu.</span><span class="sxs-lookup"><span data-stu-id="82e2b-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="82e2b-109">Vyberte **+ Přidat**.</span><span class="sxs-lookup"><span data-stu-id="82e2b-109">Select **+ Add**.</span></span> <span data-ttu-id="82e2b-110">Zaškrtněte políčko vedle názvu domény v seznamu (například contoso.com *)* a pak vyberte **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="82e2b-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="82e2b-111">Vyberte **Hotovo**.</span><span class="sxs-lookup"><span data-stu-id="82e2b-111">Select **Done**.</span></span>
- <span data-ttu-id="82e2b-112">Po vytvoření zásady můžete zásadu doladit pomocí následujících možností:</span><span class="sxs-lookup"><span data-stu-id="82e2b-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="82e2b-113">**Přidání uživatelů k ochraně:** V tomto příkladu přidejte minimálně e-mailovou adresu generálního ředitele.</span><span class="sxs-lookup"><span data-stu-id="82e2b-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="82e2b-114">**Přidání domén k ochraně:** Přidejte doménu organizace, která zahrnuje kancelář generálního ředitele.</span><span class="sxs-lookup"><span data-stu-id="82e2b-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="82e2b-115">**Zvolte akce:** Pokud  **e-mail** posílá zosobněný uživatel, vyberte Přesměrovat zprávu na jinou *e-mailovou* adresu a zadejte e-mailovou adresu správce zabezpečení (například securityadmin@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="82e2b-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="82e2b-116">V **případě, že e-mail odesílá zosobněná doména,** vyberte **Karanténa zprávy**.</span><span class="sxs-lookup"><span data-stu-id="82e2b-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="82e2b-117">**Inteligence poštovní** schránky: Ve výchozím nastavení je tato možnost vybraná při vytváření nové zásady ochrany proti phishing.</span><span class="sxs-lookup"><span data-stu-id="82e2b-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="82e2b-118">Nejlepších výsledků **dosáhnete, když** toto nastavení necháte na.</span><span class="sxs-lookup"><span data-stu-id="82e2b-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="82e2b-119">**Přidání důvěryhodných odesílatelů a domén:** V tomto příkladu nedefinujte žádné přepsání.</span><span class="sxs-lookup"><span data-stu-id="82e2b-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="82e2b-120">Po prošetřování nastavení vyberte Podle potřeby **možnost** Vytvořit tuto zásadu nebo Uložit.</span><span class="sxs-lookup"><span data-stu-id="82e2b-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="82e2b-121">Další informace najdete v tématu [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="82e2b-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
