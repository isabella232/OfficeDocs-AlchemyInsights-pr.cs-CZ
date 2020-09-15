---
title: Služba 1048 5.7.750 není dostupná. Klient blokován při posílání z neregistrovaných domén
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664235"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="93769-103">5.7.750 klienta blokován z neregistrované domény</span><span class="sxs-lookup"><span data-stu-id="93769-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="93769-104">K této chybě dojde, když je z domén, které nejsou zřízeny ve vašem tenantovi, odesílán velký objem zpráv (přidáno jako akceptované domény a jsou ověřeny).</span><span class="sxs-lookup"><span data-stu-id="93769-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="93769-105">Chcete-li se této chybě vyhnout, můžete použít konektor pro přenos pošty založený na certifikátu, ve kterém je doména certifikátu zřízená doména, nebo můžete zřídit všechny odesílající domény.</span><span class="sxs-lookup"><span data-stu-id="93769-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
