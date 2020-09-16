---
title: Oprava aplikací Microsoft 365, na které je váš účet chybný stav
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744538"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="95fc2-102">Oprava aplikací Microsoft 365 "váš účet je ve špatném stavu"</span><span class="sxs-lookup"><span data-stu-id="95fc2-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="95fc2-103">Pokud chcete chybu opravit, vyzkoušejte v příslušném počítači následující možnosti:</span><span class="sxs-lookup"><span data-stu-id="95fc2-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="95fc2-104">Otevřete aplikaci Office a vyberte **soubor**  >  **Account**  >  **Odhlásit se ze všech účtů**.</span><span class="sxs-lookup"><span data-stu-id="95fc2-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="95fc2-105">Přihlaste se znovu pomocí uživatelského účtu s platnou licencí.</span><span class="sxs-lookup"><span data-stu-id="95fc2-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="95fc2-106">Podrobné informace najdete v článku [Účty v Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="95fc2-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="95fc2-107">Pomocí Správce přihlašovacích údajů systému Windows [vymažte přihlašovací údaje Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .</span><span class="sxs-lookup"><span data-stu-id="95fc2-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="95fc2-108">**Poznámka:** Cesty registru pro Office 2016 se změnily na 16,0.</span><span class="sxs-lookup"><span data-stu-id="95fc2-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="95fc2-109">Například \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="95fc2-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="95fc2-110">Pokud dojde k chybě při připojování k Office 365 pomocí Office 2013, [Povolte moderní ověřování](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) pro klienta Office.</span><span class="sxs-lookup"><span data-stu-id="95fc2-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="95fc2-111">Další informace najdete v tématu [řešení potíží s neprohlížeči, které se nedají přihlásit k Microsoft 365, Azure nebo Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="95fc2-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

