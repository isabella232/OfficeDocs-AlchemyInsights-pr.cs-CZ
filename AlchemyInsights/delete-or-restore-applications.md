---
title: Odstranění nebo obnovení aplikací
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014750"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="e2bcc-102">Odstranění nebo obnovení aplikací</span><span class="sxs-lookup"><span data-stu-id="e2bcc-102">Delete or restore applications</span></span>

<span data-ttu-id="e2bcc-103">**Odstranění aplikace z vašeho tenanta Azure AD**:</span><span class="sxs-lookup"><span data-stu-id="e2bcc-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="e2bcc-104">Na **portálu Azure AD** vyberte **aplikace Enterprise**.</span><span class="sxs-lookup"><span data-stu-id="e2bcc-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="e2bcc-105">Pak vyhledejte a vyberte aplikaci, kterou chcete odstranit.</span><span class="sxs-lookup"><span data-stu-id="e2bcc-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="e2bcc-106">V levém podokně klikněte v části **Spravovat** na **vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="e2bcc-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="e2bcc-107">Vyberte **Odstranit** a pak kliknutím na **Ano** potvrďte, že chcete aplikaci odstranit z vašeho tenanta Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e2bcc-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="e2bcc-108">Další informace o odstranění aplikace najdete v tématu [rychlý automat: odstranění aplikace z vašeho tenanta Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="e2bcc-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="e2bcc-109">V PowerShellu rutina [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) odebere konfigurace proxy aplikací z konkrétní aplikace v Azure Active Directory a může ji úplně odstranit, pokud je zadaná.</span><span class="sxs-lookup"><span data-stu-id="e2bcc-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="e2bcc-110">**Odstraněnou aplikaci můžete obnovit** pomocí PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="e2bcc-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="e2bcc-111">Jakmile je aplikace, kterou chcete obnovit, označena, můžete ji obnovit pomocí funkce [obnovit – AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="e2bcc-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
