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
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Poradce při potížích s podpisovým certifikátem SAML

Pokud chcete vyřešit problém s podpisem SAML, postupujte podle následujících doporučených kroků:

1. Když přidáte podnikovou aplikaci, která podporuje jednotné přihlašování, Azure vygeneruje certifikát, který se nazývá [podpisový certifikát SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) Tento certifikát má datum vypršení platnosti 3 roky. Pokud chcete změnit datum vypršení platnosti certifikátu, podívejte se na část Přizpůsobení data vypršení platnosti federačního certifikátu a jeho vrácení [na nový certifikát.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)
2. Azure použije tento certifikát k podepsání tokenů SAML požadovaných aplikací a k jeho odeslání do aplikace kvůli úspěšnému jednotnému přihlašování. Aby se tento proces dokončil, stáhněte si certifikát z portálu Azure Portal a pošlete ho dodavateli aplikace, aby mohl proces jednotného přihlašování dokončit.

Po dokončení tohoto procesu bude vaše aplikace důvěřovat tomuto certifikátu a aplikaci bude akceptovat všechny tokeny SAML podepsané tímto certifikátem.

3. Pokud platnost tohoto certifikátu vyprší, vytvořte nový certifikát, aktualizujte ho u dodavatele aplikace a pak ho proveďte jako aktivní na straně Azure. Další informace najdete v článku [Prodloužení platnosti certifikátu, který brzy vyprší.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)

> [!NOTE]
> Pokud platnost certifikátu vyprší, uživatel nebude zablokovaný.

4. [Přidejte e-mailovou adresu pro](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) oznámení, která se mají dostat před vypršením platnosti aktuálního certifikátu.

> [!NOTE]
> Krok 4 je nepovinný krok.

5. Změňte možnosti podepisování certifikátu SAML aplikace a algoritmus podepisování certifikátů. Další informace najdete v článku [Změna možností podepisování certifikátů a algoritmus podepisování.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

