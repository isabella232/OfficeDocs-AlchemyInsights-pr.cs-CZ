---
title: Zařízení v Configuration Manageru chybí na portálu
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
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817237"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Zařízení v Configuration Manageru chybí na portálu

Pro fungování synchronizace je nutné, aby [požadované internetové koncové body](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) byly dostupné z místního serveru, který je hostitelem role Bod připojení služby. Pokud potřebujete vyřešit potíže se synchronizací zařízení, nahlédněte prosím do souboru **CMGatewaySyncUploadWorker.log**, který se nachází u bodu připojení služby.

Přečtěte si další informace o [připojení tenanta v Microsoft Endpoint Manageru](https://docs.microsoft.com/configmgr/tenant-attach/).
