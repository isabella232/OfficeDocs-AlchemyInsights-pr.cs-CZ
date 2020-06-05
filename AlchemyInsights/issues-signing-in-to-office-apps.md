---
title: Problémy s přihlášením k aplikacím Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579930"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="8e247-102">Oprava zprávy Aplikace Microsoft 365 "Omlouváme se, jiný účet z vaší organizace je již přihlášen"</span><span class="sxs-lookup"><span data-stu-id="8e247-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="8e247-103">Pokud chcete tuto chybu vyřešit, vyzkoušejte následující:</span><span class="sxs-lookup"><span data-stu-id="8e247-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="8e247-104">Odeberte všechny pracovní účty kromě ovlivněného účtu pomocí nastavení Windows > **práce nebo školy aplikace Access**.</span><span class="sxs-lookup"><span data-stu-id="8e247-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="8e247-105">[Vymazání přihlašovacích údajů Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocí Správce pověření systému Windows</span><span class="sxs-lookup"><span data-stu-id="8e247-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="8e247-106">**Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0.</span><span class="sxs-lookup"><span data-stu-id="8e247-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="8e247-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="8e247-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="8e247-108">Otevřete aplikaci Office a zvolte **Odhlásit se**  >  **na účet**souborů  >  **Sign Out**. Pak se přihlaste pomocí uživatelského účtu s platnou licencí.</span><span class="sxs-lookup"><span data-stu-id="8e247-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="8e247-109">Podrobné informace najdete v článku [Účty v Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="8e247-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="8e247-110">V případě Macu si projděte téma [Nejde se přihlásit k aplikaci Office 2016 pro Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="8e247-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="8e247-111">Další informace naleznete [v tématu "Omlouváme se, jiný účet z vaší organizace je již přihlášen k tomuto počítači" v office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="8e247-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>