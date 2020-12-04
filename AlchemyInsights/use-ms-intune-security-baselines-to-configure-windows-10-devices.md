---
title: Konfigurace zařízení s Windows 10 pomocí standardních hodnot zabezpečení Microsoft Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573332"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Konfigurace zařízení s Windows 10 pomocí standardních hodnot zabezpečení Microsoft Intune

Plány zabezpečení Intune pomáhají chránit uživatele a zařízení. Směrné plány zabezpečení: nastavení systému Windows – předdefinované skupiny používané k použití známé skupiny nastavení a výchozích hodnot doporučených příslušnými týmy zabezpečení. Vytvořením profilu zabezpečení podle směrného plánu v Intune vytvoříte šablonu, která se skládá z více konfiguračních profilů zařízení.

Při nasazení standardních hodnot zabezpečení do skupin uživatelů nebo zařízení se nastavení aplikuje na zařízení, která běží ve Windows 10 nebo novějším. Například automatické přizpůsobení úrovně zabezpečení MDM (1) umožňuje BitLocker pro vyměnitelné jednotky (2) vyžaduje heslo pro odemknutí zařízení a (3) zakáže základní ověřování. Pokud ve vašem prostředí nefunguje výchozí hodnota, upravte podle směrného plánu požadované nastavení.

Směrné plány zabezpečení pomáhají také při vytvoření zabezpečeného pracovního postupu v Microsoft 365. Tady jsou některé výhody:

- Směrný plán zabezpečení obsahuje osvědčené postupy a doporučení pro nastavení, která ovlivňují zabezpečení. Vzhledem k tomu, že partneři Intune se skupinou zabezpečení systému Windows, které vytvářejí směrné plány pro zásady skupiny, tato doporučení vycházejí z plných pokynů a rozsáhlých zkušeností.
- Pokud se chystáte s Intune a nejste si jistí, kde začít, pak vám směrné plány zabezpečení umožní rychle vytvořit a nasadit zabezpečený profil.
- Pokud v současné době používáte zásady skupiny, je migrace na Intune pro účely správy mnohem snadnější díky základním hodnotám zabezpečení, protože jsou integrované do Intune a zahrnují pro správu možnosti vyjímání.

Další informace najdete v tématu [směrné plány zabezpečení Windows](https://go.microsoft.com/fwlink/?linkid=2141503) a [Správa mobilních zařízení](https://go.microsoft.com/fwlink/?linkid=2141701).