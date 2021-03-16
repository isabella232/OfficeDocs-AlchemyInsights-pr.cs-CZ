---
title: Řešení potíží s jednotným přihlašováním (SSO) pro místní nasazení
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816092"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="0c85b-102">Řešení potíží s jednotným přihlašováním (SSO) pro místní nasazení</span><span class="sxs-lookup"><span data-stu-id="0c85b-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="0c85b-103">Pokud chcete vyřešit bezproblémové problémy s jednotným přihlašováním (SSO), postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="0c85b-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="0c85b-104">**Jak můžu přetáhnout dešifrovací klíč Kerberos účtu počítače AZUREADSSO?**</span><span class="sxs-lookup"><span data-stu-id="0c85b-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="0c85b-105">Důrazně doporučujeme, abyste dešifrovací klíč Kerberos přehodíte aspoň každých 30 dní.</span><span class="sxs-lookup"><span data-stu-id="0c85b-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="0c85b-106">Pokud to chcete udělat ručně, podívejte se na postup [převrácení dešifrovací klávesy Kerberos.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#)</span><span class="sxs-lookup"><span data-stu-id="0c85b-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="0c85b-107">**Konfigurace bezproblémového jednotného přihlašování**</span><span class="sxs-lookup"><span data-stu-id="0c85b-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="0c85b-108">Pokud chcete nasadit bezproblémové jednotné přihlašování, postupujte podle pokynů v tématu Bezproblémové jednotné přihlašování [v Azure Active Directory: Rychlý start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span><span class="sxs-lookup"><span data-stu-id="0c85b-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="0c85b-109">**Doporučení**</span><span class="sxs-lookup"><span data-stu-id="0c85b-109">**Advisory**</span></span>

- <span data-ttu-id="0c85b-110">[Bezproblémové](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) jednotné přihlašování k Azure Active Directory: Nejčastější dotazy – v tomto článku řešíme časté otázky k Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span><span class="sxs-lookup"><span data-stu-id="0c85b-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="0c85b-111">Pokračujte v kontrole nového obsahu.</span><span class="sxs-lookup"><span data-stu-id="0c85b-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="0c85b-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) – Tento článek obsahuje informace o tom, jak vytvořit žádosti o funkce nebo se zeptat na technické otázky týkající se bezproblémového jednotného přihlašování.</span><span class="sxs-lookup"><span data-stu-id="0c85b-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="0c85b-113">**Řešení potíží**</span><span class="sxs-lookup"><span data-stu-id="0c85b-113">**Troubleshoot**</span></span>

<span data-ttu-id="0c85b-114">[Řešení potíží s bezproblémovým](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) jednotným přihlašováním k Azure Active Directory – tento článek vám pomůže najít informace o řešení běžných problémů týkajících se Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span><span class="sxs-lookup"><span data-stu-id="0c85b-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







