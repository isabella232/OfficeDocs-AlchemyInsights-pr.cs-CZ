---
title: Více objektů má stejnou e-mailovou adresu jako identita
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724608"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="993d0-102">Více objektů má stejnou e-mailovou adresu jako identita</span><span class="sxs-lookup"><span data-stu-id="993d0-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="993d0-103">**Více objektů**</span><span class="sxs-lookup"><span data-stu-id="993d0-103">**Multiple objects**</span></span>

<span data-ttu-id="993d0-104">Jedním ze častých důvodů této chyby není umožnit správné směrování požadavku aplikace Outlook Web Access v přítomnosti více objektů se stejnou e-mailovou adresou jako identita.</span><span class="sxs-lookup"><span data-stu-id="993d0-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="993d0-105">K vyhledání těchto objektů použijte následující příkazy:</span><span class="sxs-lookup"><span data-stu-id="993d0-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="993d0-106">· Get-příjemce <email address></span><span class="sxs-lookup"><span data-stu-id="993d0-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="993d0-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="993d0-107">· Get-User <email address></span></span>

<span data-ttu-id="993d0-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="993d0-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="993d0-109">· Získat kontakt <email address></span><span class="sxs-lookup"><span data-stu-id="993d0-109">· Get-Contact <email address></span></span>

<span data-ttu-id="993d0-110">· Get – poštovní schránka <email address> – PublicFolder</span><span class="sxs-lookup"><span data-stu-id="993d0-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="993d0-111">· Get – poštovní schránka <email address> – IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="993d0-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="993d0-112">· Get – poštovní schránka <email address> – InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="993d0-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="993d0-113">Tento problém vyřešíte tak, že odeberete více objektů se stejnou e-mailovou identitou a zajistěte, aby byl jediný objekt se specifickou identitou e-mailu a aby jeho typ příjemce byl UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="993d0-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="993d0-114">**Pro firemní a spotřebitelské poštovní schránky se používá stejná adresa**</span><span class="sxs-lookup"><span data-stu-id="993d0-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="993d0-115">Další příčina je, když se pro firemní a spotřebitelské poštovní schránky používá stejná adresa.</span><span class="sxs-lookup"><span data-stu-id="993d0-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="993d0-116">V tomto případě musí uživatel změnit svůj primární alias pro uživatele, dokud kavárny tento scénář nepodporuje.</span><span class="sxs-lookup"><span data-stu-id="993d0-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="993d0-117">Jedná se o trvalou chybu, která není bez zásahu.</span><span class="sxs-lookup"><span data-stu-id="993d0-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="993d0-118">Podrobnosti najdete v článku [Změna e-mailové adresy nebo telefonního čísla pro váš účet Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="993d0-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>