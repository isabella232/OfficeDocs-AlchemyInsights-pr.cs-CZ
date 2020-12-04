---
title: Rozšířené principy ověřování vztahující se na Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573329"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="cac3f-102">Rozšířené principy ověřování vztahující se na Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="cac3f-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="cac3f-103">Následují rozšířené principy ověřování, které platí pro Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="cac3f-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="cac3f-104">**Proaktivní ověřování**</span><span class="sxs-lookup"><span data-stu-id="cac3f-104">**Proactive Authentication**</span></span>

<span data-ttu-id="cac3f-105">Když povolíte zásadu [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge se pokusí aktivně ověřovat přihlášené uživatele prostřednictvím služeb Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="cac3f-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="cac3f-106">V pravidelných intervalech se pomocí online služby vyhledá aktualizovaný manifest, který obsahuje konfiguraci aktivního ověřování.</span><span class="sxs-lookup"><span data-stu-id="cac3f-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="cac3f-107">Výhody: proaktivní ověřování umožňuje ověřování pro klíčové služby, jako je třeba stránka nové karty Office.</span><span class="sxs-lookup"><span data-stu-id="cac3f-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="cac3f-108">Pokud se jako vyhledávací stroj používá Bing, proaktivní ověřování zlepšuje výkon panelu Adresa a pomáhá vytvářet výsledky hledání podle potřeb vaší firmy.</span><span class="sxs-lookup"><span data-stu-id="cac3f-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="cac3f-109">**Windows Hello pro CredUI pro ověřování NTLM**</span><span class="sxs-lookup"><span data-stu-id="cac3f-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="cac3f-110">Pokud není k dispozici jednotné přihlašování (SSO), když se web pokusí přihlásit k uživateli prostřednictvím mechanismu NTLM nebo Negotiate, umožní vám tato funkce sdílet přihlašovací údaje operačního systému s webem a splnit ověřovací výzvu pomocí přihlašovacího uživatelského rozhraní Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="cac3f-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="cac3f-111">Tento tok přihlašování se zobrazí jenom ve Windows 10 a jenom uživatelům, kteří nezískají jednotné přihlašování v průběhu ověřování NTLM nebo vyjednávání.</span><span class="sxs-lookup"><span data-stu-id="cac3f-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="cac3f-112">**Automatické přihlašování pomocí uložených hesel**</span><span class="sxs-lookup"><span data-stu-id="cac3f-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="cac3f-113">Uživatelé, kteří ukládají hesla v Microsoft Edge, můžou povolit automatické přihlašování k webům, kde mají uložená přihlašovací údaje.</span><span class="sxs-lookup"><span data-stu-id="cac3f-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="cac3f-114">Uživatelé můžou tuto funkci zapnout nebo vypnout v edge://settings/passwords a nakonfigurovat ji v zásadách [správce hesel](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="cac3f-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
