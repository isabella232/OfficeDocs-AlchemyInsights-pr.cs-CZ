---
title: 'Oprava aplikací Microsoft 365: Váš účet je ve špatném stavu'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812529"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="26143-102">Oprava chyby aplikace Microsoft 365 "Váš účet je ve špatném stavu".</span><span class="sxs-lookup"><span data-stu-id="26143-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="26143-103">Pokud chcete tuto chybu vyřešit, vyzkoušejte na příslušném počítači následující možnosti:</span><span class="sxs-lookup"><span data-stu-id="26143-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="26143-104">Otevřete aplikaci Office a vyberte  >  **Souborový účet**  >  **Odhlásit se ze všech účtů**.</span><span class="sxs-lookup"><span data-stu-id="26143-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="26143-105">Přihlaste se znovu pomocí uživatelského účtu s platnou licencí.</span><span class="sxs-lookup"><span data-stu-id="26143-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="26143-106">Podrobné informace najdete v článku [Účty v Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="26143-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="26143-107">[Vymažte přihlašovací údaje Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocí Správce přihlašovacích údajů systému Windows.</span><span class="sxs-lookup"><span data-stu-id="26143-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="26143-108">**Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0.</span><span class="sxs-lookup"><span data-stu-id="26143-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="26143-109">Například \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="26143-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="26143-110">Pokud k chybě dojde při připojování k Office 365 pomocí Office 2013, [povolte](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) moderní ověřování pro klienta Office.</span><span class="sxs-lookup"><span data-stu-id="26143-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="26143-111">Další informace najdete v článku Řešení potíží s aplikacemi mimo prohlížeč, které se neschytá přihlásit k [Microsoftu 365, Azure](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)nebo Intune.</span><span class="sxs-lookup"><span data-stu-id="26143-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

