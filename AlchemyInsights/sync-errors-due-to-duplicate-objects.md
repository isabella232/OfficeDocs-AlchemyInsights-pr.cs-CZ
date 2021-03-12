---
title: 902 (Chyby synchronizace kvůli duplicitním objektům)
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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708055"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="b10a2-102">Chyby synchronizace kvůli duplicitním objektům</span><span class="sxs-lookup"><span data-stu-id="b10a2-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="b10a2-103">Po dokončení synchronizace adresářů v Microsoftu 365 se může zobrazit jedna z následujících chybových zpráv:</span><span class="sxs-lookup"><span data-stu-id="b10a2-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="b10a2-104">Tento objekt nelze aktualizovat ve službách Microsoft Online Services, protože následující atributy přidružené k tomuto objektu mají hodnoty, které mohou být již přidruženy k jinému objektu v místním adresáři.</span><span class="sxs-lookup"><span data-stu-id="b10a2-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="b10a2-105">Synchronizovaný objekt se stejnou adresou proxy serveru už v adresáři služeb Microsoft Online Services existuje.</span><span class="sxs-lookup"><span data-stu-id="b10a2-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="b10a2-106">Tento objekt nelze aktualizovat, protože následující atributy přidružené k tomuto objektu mají hodnoty, které již mohou být přidruženy k jinému objektu v místních adresářových službách: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="b10a2-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="b10a2-107">Pokud chcete tento problém identifikovat a opravit, stáhněte a spusťte Nástroj [IdFix DirSync Error Remediation Tool.](https://github.com/Microsoft/idfix)</span><span class="sxs-lookup"><span data-stu-id="b10a2-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="b10a2-108">Další informace najdete v [článku KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)</span><span class="sxs-lookup"><span data-stu-id="b10a2-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
