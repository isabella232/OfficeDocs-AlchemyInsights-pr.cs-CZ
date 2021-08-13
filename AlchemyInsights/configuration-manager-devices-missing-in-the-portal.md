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
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966102"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Zařízení v Configuration Manageru chybí na portálu

Pro fungování synchronizace je nutné, aby [požadované internetové koncové body](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) byly dostupné z místního serveru, který je hostitelem role Bod připojení služby. Pokud potřebujete vyřešit potíže se synchronizací zařízení, nahlédněte prosím do souboru **CMGatewaySyncUploadWorker.log**, který se nachází u bodu připojení služby.

Přečtěte si další informace o [připojení tenanta v Microsoft Endpoint Manageru](https://docs.microsoft.com/configmgr/tenant-attach/).
