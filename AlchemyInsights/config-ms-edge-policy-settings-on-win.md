---
title: Konfigurace nastavení zásad Microsoft Edge ve Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "9004632"
- "6894"
- "8358"
ms.openlocfilehash: e9bb489b4d8ecd76fd777ade9fb740ecad542900
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402368"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="229cf-102">Konfigurace nastavení zásad Microsoft Edge ve Windows</span><span class="sxs-lookup"><span data-stu-id="229cf-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="229cf-103">Pokud chcete nakonfigurovat nastavení zásad a spravované aktualizace pro Microsoft Edge, použijte Zásady skupiny objekty zásad skupiny.</span><span class="sxs-lookup"><span data-stu-id="229cf-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="229cf-104">Zásady můžete také zřídit prostřednictvím registru. to by bylo vhodné pro (1) zařízení s Windows připojená k doméně služba Microsoft Active Directory a pro (2) instance Windows 10 Pro a Enterprise zaregistrovaná pro správu zařízení v Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="229cf-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="229cf-105">Pokud chcete nakonfigurovat Microsoft Edge pomocí objektů zásad skupiny, proveďte toto:</span><span class="sxs-lookup"><span data-stu-id="229cf-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="229cf-106">Přejděte do centrálního úložiště Zásady skupiny ve vaší doméně služby Active Directory nebo do složky šablon Definice zásad na jednotlivých počítačích a nainstalujte všechny šablony pro správu, které přidávají pravidla a nastavení pro Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="229cf-106">Go to the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="229cf-107">Nakonfigurujte konkrétní zásady, které chcete nastavit.</span><span class="sxs-lookup"><span data-stu-id="229cf-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="229cf-108">Další informace najdete v tématu [Konfigurace nastavení zásad Microsoft Edge ve Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span><span class="sxs-lookup"><span data-stu-id="229cf-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
