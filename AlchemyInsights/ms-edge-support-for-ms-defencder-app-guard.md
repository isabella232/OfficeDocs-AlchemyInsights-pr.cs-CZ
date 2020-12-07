---
title: Podpora Microsoftu pro Microsoft Edge pro ochranu Application Guard
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
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583366"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Podpora Microsoftu pro Microsoft Edge pro ochranu Application Guard

Pro Windows 10 a Microsoft Edge používá funkce Guard přístup k izolaci hardwaru, pomocí kterého může uživatel přejít na nedůvěryhodný web z izolovaného kontejneru povoleného technologií Hyper-V, který je oddělen od hostitelského operačního systému.

Správce rozlehlé sítě definuje seznam důvěryhodných webů, cloudových zdrojů a interních sítí. Když uživatel navštíví web, který není v seznamu, otevře Microsoft Edge Web v kontejneru. To znamená, že pokud se web vypíná za nebezpečný, bude hostitelský počítač i nadále chráněn a útočník se nedostane do podnikových dat.

Instalace rozšíření v kontejneru je podporovaná od Microsoft Edge verze 81 a dá se ovládat prostřednictvím zásad. Adresa updateURL, která se používá v zásadách ExtensionInstallForcelist, by se měla přidat jako neutrální prostředek do zásad izolace sítě používaných ochranou Application Guard.

Další informace najdete v článku [Podpora Microsoft Edge pro ochranu Application Guard pro Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2134229).
