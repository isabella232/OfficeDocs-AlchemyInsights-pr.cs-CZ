---
title: Poradce při potížích s podpisovým certifikátem SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692653"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="d2f82-102">Poradce při potížích s podpisovým certifikátem SAML</span><span class="sxs-lookup"><span data-stu-id="d2f82-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="d2f82-103">Pokud chcete vyřešit problém s podpisem SAML, postupujte podle následujících doporučených kroků:</span><span class="sxs-lookup"><span data-stu-id="d2f82-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="d2f82-104">Když přidáte podnikovou aplikaci, která podporuje jednotné přihlašování, Azure vygeneruje certifikát, který se nazývá [podpisový certifikát SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="d2f82-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="d2f82-105">Tento certifikát má datum vypršení platnosti 3 roky.</span><span class="sxs-lookup"><span data-stu-id="d2f82-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="d2f82-106">Pokud chcete změnit datum vypršení platnosti certifikátu, podívejte se na část Přizpůsobení data vypršení platnosti federačního certifikátu a jeho vrácení [na nový certifikát.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)</span><span class="sxs-lookup"><span data-stu-id="d2f82-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="d2f82-107">Azure použije tento certifikát k podepsání tokenů SAML požadovaných aplikací a k jeho odeslání do aplikace kvůli úspěšnému jednotnému přihlašování.</span><span class="sxs-lookup"><span data-stu-id="d2f82-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="d2f82-108">Aby se tento proces dokončil, stáhněte si certifikát z portálu Azure Portal a pošlete ho dodavateli aplikace, aby mohl proces jednotného přihlašování dokončit.</span><span class="sxs-lookup"><span data-stu-id="d2f82-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="d2f82-109">Po dokončení tohoto procesu bude vaše aplikace důvěřovat tomuto certifikátu a aplikaci bude akceptovat všechny tokeny SAML podepsané tímto certifikátem.</span><span class="sxs-lookup"><span data-stu-id="d2f82-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="d2f82-110">Pokud platnost tohoto certifikátu vyprší, vytvořte nový certifikát, aktualizujte ho u dodavatele aplikace a pak ho proveďte jako aktivní na straně Azure.</span><span class="sxs-lookup"><span data-stu-id="d2f82-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="d2f82-111">Další informace najdete v článku [Prodloužení platnosti certifikátu, který brzy vyprší.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)</span><span class="sxs-lookup"><span data-stu-id="d2f82-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="d2f82-112">Pokud platnost certifikátu vyprší, uživatel nebude zablokovaný.</span><span class="sxs-lookup"><span data-stu-id="d2f82-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="d2f82-113">[Přidejte e-mailovou adresu pro](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) oznámení, která se mají dostat před vypršením platnosti aktuálního certifikátu.</span><span class="sxs-lookup"><span data-stu-id="d2f82-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="d2f82-114">Krok 4 je nepovinný krok.</span><span class="sxs-lookup"><span data-stu-id="d2f82-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="d2f82-115">Změňte možnosti podepisování certifikátu SAML aplikace a algoritmus podepisování certifikátů.</span><span class="sxs-lookup"><span data-stu-id="d2f82-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="d2f82-116">Další informace najdete v článku [Změna možností podepisování certifikátů a algoritmus podepisování.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="d2f82-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

