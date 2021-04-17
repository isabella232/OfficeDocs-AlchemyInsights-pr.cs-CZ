---
title: Chyby při vytváření živých událostí v Yammeru
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
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825508"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="b4d24-102">Chyby při vytváření živých událostí v Yammeru</span><span class="sxs-lookup"><span data-stu-id="b4d24-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="b4d24-103">**Vytvoření živé události v Yammeru**</span><span class="sxs-lookup"><span data-stu-id="b4d24-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="b4d24-104">Yammer vždy zobrazuje možnost vytvoření živé události.</span><span class="sxs-lookup"><span data-stu-id="b4d24-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="b4d24-105">V některých případech ale uživatel nemusí splňovat požadavky pro vytvoření živé události a při pokusu o její vytvoření může dojít k chybě.</span><span class="sxs-lookup"><span data-stu-id="b4d24-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="b4d24-106">Níže uvedené položky popisují časté důvody pro vznik tohoto problému a poskytují způsoby jeho řešení pro koncové uživatele.</span><span class="sxs-lookup"><span data-stu-id="b4d24-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="b4d24-107">**Kdo může vytvářet živé události**</span><span class="sxs-lookup"><span data-stu-id="b4d24-107">**Who can create live events**</span></span>
- <span data-ttu-id="b4d24-108">Licence Office 365 Enterprise E1, E3 nebo E5 nebo licence Office 365 A3 nebo A5.</span><span class="sxs-lookup"><span data-stu-id="b4d24-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="b4d24-109">Oprávnění vytvářet živé události v centru pro správu Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b4d24-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="b4d24-110">Oprávnění vytvářet živé události v Microsoft Streamu (pro události produkované prostřednictvím externí vysílací aplikace nebo zařízení).</span><span class="sxs-lookup"><span data-stu-id="b4d24-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="b4d24-111">Plné týmové členství v organizaci (nemůže to být host ani osoba z jiné organizace).</span><span class="sxs-lookup"><span data-stu-id="b4d24-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="b4d24-112">Aktivované plánování soukromých schůzek, sdílení obrazovky a sdílení IP videa v zásadách týmových schůzek.</span><span class="sxs-lookup"><span data-stu-id="b4d24-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="b4d24-113">**Zásady vytváření živé události**</span><span class="sxs-lookup"><span data-stu-id="b4d24-113">**Live event creation policies**</span></span>

<span data-ttu-id="b4d24-114">Yammer se řídí zásadami živých událostí, které jsou nastavené ve vašem tenantovi Office 365 pro Stream.</span><span class="sxs-lookup"><span data-stu-id="b4d24-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="b4d24-115">Ve výchozím nastavení může živé události vytvářet kdokoli v organizaci.</span><span class="sxs-lookup"><span data-stu-id="b4d24-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="b4d24-116">Správci můžou [toto nastavení změnit, což může uživatelům bránit ve vytvoření živé události](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="b4d24-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="b4d24-117">V případě, že se při vytváření živé události objeví chyba zásady, je důležité zkontrolovat, jestli mají uživatelé oprávnění živé události vytvářet.</span><span class="sxs-lookup"><span data-stu-id="b4d24-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
