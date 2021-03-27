---
title: Pokročilé koncepty ověřování platné pro Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398548"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="07330-102">Pokročilé koncepty ověřování platné pro Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="07330-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="07330-103">Tady jsou pokročilé koncepty ověřování, které se vztahují na Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="07330-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="07330-104">**Proaktivní ověřování**</span><span class="sxs-lookup"><span data-stu-id="07330-104">**Proactive Authentication**</span></span>

<span data-ttu-id="07330-105">Když povolíte zásadu [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge se pokusí proaktivně ověřovat přihlášené uživatele prostřednictvím služeb Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="07330-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="07330-106">V pravidelných intervalech bude používat online službu ke kontrole aktualizovaného manifestu, který obsahuje konfiguraci, která řídí proaktivní ověřování.</span><span class="sxs-lookup"><span data-stu-id="07330-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="07330-107">Výhody: Proaktivní ověřování umožňuje ověřování klíčových služeb, jako je například stránka Nové karty Office.</span><span class="sxs-lookup"><span data-stu-id="07330-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="07330-108">Pokud se jako vyhledávací modul používá Bing, zlepšuje proaktivní ověřování výkon panelu Adresa a pomáhá generovat výsledky hledání přizpůsobené potřebám vaší firmy.</span><span class="sxs-lookup"><span data-stu-id="07330-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="07330-109">**Windows Hello CredUI pro ověřování NTLM**</span><span class="sxs-lookup"><span data-stu-id="07330-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="07330-110">Pokud jednotné přihlašování (SSO) není dostupné, když se web pokusí přihlásit k uživateli pomocí mechanizmu NTLM nebo Vyjednat, umožní tato funkce uživateli sdílet přihlašovací údaje operačního systému s webem a vyhovět výzvě při ověřování pomocí uživatelského rozhraní Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="07330-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="07330-111">Tento tok přihlašování se zobrazí jenom ve Windows 10 a jenom pro uživatele, kteří nezísknou jednotné přihlašování během výzvy NTLM nebo Vyjednat.</span><span class="sxs-lookup"><span data-stu-id="07330-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="07330-112">**Automatické přihlašování pomocí uložených hesel**</span><span class="sxs-lookup"><span data-stu-id="07330-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="07330-113">Uživatelé, kteří ukládají hesla v Microsoft Edgi, mohou povolit automatické přihlašování k webům, kde mají uložené přihlašovací údaje.</span><span class="sxs-lookup"><span data-stu-id="07330-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="07330-114">Uživatelé mohou tuto funkci zapnout nebo vypnout v edge://settings/passwords a můžete ji nakonfigurovat v zásadách [správce](https://go.microsoft.com/fwlink/?linkid=2134622) hesel.</span><span class="sxs-lookup"><span data-stu-id="07330-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
