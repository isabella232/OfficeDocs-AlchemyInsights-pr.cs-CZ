---
title: Více objektů má stejnou e-mailovou adresu jako identita
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438800"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="a33c6-102">Více objektů má stejnou e-mailovou adresu jako identita</span><span class="sxs-lookup"><span data-stu-id="a33c6-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="a33c6-103">**Více objektů**</span><span class="sxs-lookup"><span data-stu-id="a33c6-103">**Multiple objects**</span></span>

<span data-ttu-id="a33c6-104">Jedním z běžných důvodů této chyby není možnost správně směrovat požadavek aplikace Outlook Web Access v přítomnosti více objektů, které mají stejnou e-mailovou adresu jako identita.</span><span class="sxs-lookup"><span data-stu-id="a33c6-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="a33c6-105">Chcete-li tyto objekty najít, spusťte následující příkazy:</span><span class="sxs-lookup"><span data-stu-id="a33c6-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="a33c6-106">· Příjemce<email address></span><span class="sxs-lookup"><span data-stu-id="a33c6-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="a33c6-107">· Získat uživatele<email address></span><span class="sxs-lookup"><span data-stu-id="a33c6-107">· Get-User <email address></span></span>

<span data-ttu-id="a33c6-108">· Get-User <email address> -SoftDeleteduser</span><span class="sxs-lookup"><span data-stu-id="a33c6-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="a33c6-109">· Získat kontakt<email address></span><span class="sxs-lookup"><span data-stu-id="a33c6-109">· Get-Contact <email address></span></span>

<span data-ttu-id="a33c6-110">· Poštovní <email address> schránka -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="a33c6-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="a33c6-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="a33c6-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="a33c6-112">· Get-Mailbox <email address> -NeaktivníMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="a33c6-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="a33c6-113">Chcete-li tento problém vyřešit, odeberte více objektů se stejnou identitou e-mailu a ujistěte se, že existuje jeden objekt s konkrétní identitou e-mailu a že jeho typ příjemce je UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="a33c6-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="a33c6-114">**Stejná adresa se používá pro obchodní a spotřebitelské poštovní schránky**</span><span class="sxs-lookup"><span data-stu-id="a33c6-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="a33c6-115">Další příčinou je, když se stejná adresa používá pro obchodní a spotřebitelské poštovní schránky.</span><span class="sxs-lookup"><span data-stu-id="a33c6-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="a33c6-116">V takovém případě musí uživatel změnit svůj primární prostředek příjemce alias, dokud Kavárna podporuje tento scénář.</span><span class="sxs-lookup"><span data-stu-id="a33c6-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="a33c6-117">Jedná se o trvalou chybu, která nezmizí bez zásahu.</span><span class="sxs-lookup"><span data-stu-id="a33c6-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="a33c6-118">Podrobnosti najdete [v tématu Změna e-mailové adresy nebo telefonního čísla účtu Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="a33c6-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>