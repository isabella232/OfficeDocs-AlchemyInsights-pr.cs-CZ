---
title: Řešení problému – uživatel nebyl nalezen v adresáři
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725400"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="f8444-102">Řešení problému – uživatel nebyl nalezen v adresáři</span><span class="sxs-lookup"><span data-stu-id="f8444-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="f8444-103">Pokud se uživatelům zobrazí chybová zpráva "uživatel nebyl nalezen" v adresáři, zkuste to znovu, kde typ problému uživatel není v adresáři.</span><span class="sxs-lookup"><span data-stu-id="f8444-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="f8444-104">Tento problém můžete vyřešit provedením následujících kroků.</span><span class="sxs-lookup"><span data-stu-id="f8444-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="f8444-105">Ujistěte se, že účet, který přijal pozvánku, je stejný účet, který se používá k pozdějšímu přihlášení.</span><span class="sxs-lookup"><span data-stu-id="f8444-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="f8444-106">Ujistěte se, že uživatel používá stejný účet pro přijetí pozvánky a přihlášení na web.</span><span class="sxs-lookup"><span data-stu-id="f8444-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="f8444-107">Další informace najdete v tématu [jak spravovat aliasy pro váš účet Microsoft </a> pro správu přihlášení Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="f8444-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="f8444-108">Přejděte na jednotlivé weby, ve kterých uživatel obdrží chybu.</span><span class="sxs-lookup"><span data-stu-id="f8444-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="f8444-109">Add "/_layouts/15/People.aspx/MembershipGroupId = 0" (uvnitř uvozovek) na konec adresy URL webu.</span><span class="sxs-lookup"><span data-stu-id="f8444-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="f8444-110">Příklad: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="f8444-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="f8444-111">Vyberte uživatele ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="f8444-111">Select the user from the list.</span></span>

- <span data-ttu-id="f8444-112">Na pásu karet klikněte na **Odebrat uživatelská oprávnění** .</span><span class="sxs-lookup"><span data-stu-id="f8444-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="f8444-113">Přidat uživatele a znovu odeslat pozvánku uživateli</span><span class="sxs-lookup"><span data-stu-id="f8444-113">Add back the User and Resend the invite to the user.</span></span>

