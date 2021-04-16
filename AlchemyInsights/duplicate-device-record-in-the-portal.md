---
title: Duplicitní záznam zařízení na portálu.
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814509"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="b2621-102">Duplicitní záznam zařízení na portálu.</span><span class="sxs-lookup"><span data-stu-id="b2621-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="b2621-103">Pokud zařízení nehlásí správný přehled o stavu na stránce Správce konfigurace, můžou se vám na portálu zobrazovat dva záznamy. </span><span class="sxs-lookup"><span data-stu-id="b2621-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="b2621-104">Pokud chcete zkontrolovat stav konkrétního zařízení, podívejte se do sloupce **Spoluspravované** na zařízení v konzole Správce konfigurace.</span><span class="sxs-lookup"><span data-stu-id="b2621-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="b2621-105">Pokud není sloupec zobrazený, můžete ho přidat kliknutím pravým tlačítkem myši na záhlaví sloupce a vybrat ho ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="b2621-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="b2621-106">Spoluspravovaná hodnota musí být **Ano**.</span><span class="sxs-lookup"><span data-stu-id="b2621-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="b2621-107">Pokud je hodnota **Ne**, otevřete na klientském zařízení aplet Správce konfigurace a zkontrolujte **vlastnosti spolusprávy** na kartě Obecné.</span><span class="sxs-lookup"><span data-stu-id="b2621-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="b2621-108">Pokud je hodnota **Povolena**, znamená to, že se jedná o problémy komunikace klienta s bodem správy.</span><span class="sxs-lookup"><span data-stu-id="b2621-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="b2621-109">Abyste mohli prozkoumat potenciální problémy s připojením, podívejte se prosím na **CcmMessaging. log** na zařízení.</span><span class="sxs-lookup"><span data-stu-id="b2621-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="b2621-110">Pokud je hodnota **Zakázaná** a zařízení se registruje v Intune, ujistěte se prosím, že zařízení dostalo zásadu pro spolusprávu, a to tak, že na zařízení zkontrolujete **CoManagementHandler.log.**</span><span class="sxs-lookup"><span data-stu-id="b2621-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
