---
title: Řešení potíží s souhlasem uživatele
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900959"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="ad5df-102">Řešení potíží s souhlasem uživatele</span><span class="sxs-lookup"><span data-stu-id="ad5df-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="ad5df-103">Můžete nakonfigurovat, jak budou koncoví uživatelé souhlasit s aplikacemi prostřednictvím portálu Azure nebo PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="ad5df-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="ad5df-104">Další informace najdete v článku [nastavení souhlasu uživatele](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .</span><span class="sxs-lookup"><span data-stu-id="ad5df-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="ad5df-105">Správce může také použít [rozhraní Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) k udělení souhlasu jménem jednoho uživatele.</span><span class="sxs-lookup"><span data-stu-id="ad5df-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="ad5df-106">Další informace najdete v článku o [získání přístupu v zastoupení uživatele](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="ad5df-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="ad5df-107">[Chyby souhlasu uživatelů](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): Tento článek popisuje chyby, ke kterým může dojít při procesu přijetí do aplikace.</span><span class="sxs-lookup"><span data-stu-id="ad5df-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="ad5df-108">Pokud chcete řešit potíže s neočekávanými zprávami o souhlasu, které neobsahují žádné chybové zprávy, přečtěte si článek [scénáře ověřování pro Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="ad5df-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>