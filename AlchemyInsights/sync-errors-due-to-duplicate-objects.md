---
title: 902 (chyby synchronizace kvůli duplicitním objektům)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737334"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="5bd54-102">Chyby synchronizace kvůli duplicitním objektům</span><span class="sxs-lookup"><span data-stu-id="5bd54-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="5bd54-103">Při dokončení synchronizace adresáře v Microsoft 365 se může zobrazit jedna z následujících chybových zpráv:</span><span class="sxs-lookup"><span data-stu-id="5bd54-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="5bd54-104">Tento objekt nejde aktualizovat v online službách Microsoftu, protože následující atributy přidružené k tomuto objektu mají hodnoty, které už můžou být přidružené k jinému objektu v místním adresáři.</span><span class="sxs-lookup"><span data-stu-id="5bd54-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="5bd54-105">Synchronizovaný objekt se stejnou proxy adresou už v adresáři služeb Microsoft Online Services existuje.</span><span class="sxs-lookup"><span data-stu-id="5bd54-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="5bd54-106">Tento objekt nejde aktualizovat, protože následující atributy přidružené k tomuto objektu mají hodnoty, které už můžou být přidružené k jinému objektu v místních adresářových službách: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="5bd54-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="5bd54-107">Chcete-li zjistit a opravit problém, Stáhněte a spusťte [Nástroj IdFix DirSync chyby](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="5bd54-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="5bd54-108">Další informace najdete v tématu [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="5bd54-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
