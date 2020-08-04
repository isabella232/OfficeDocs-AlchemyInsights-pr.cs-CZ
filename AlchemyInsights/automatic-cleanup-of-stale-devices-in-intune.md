---
title: Automatické vyčištění zastaralých zařízení v Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554836"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatické vyčištění zastaralých zařízení v Intune

Intune umožňuje správci konfigurovat časový interval mezi 90 a 270 dny, po kterém se ze služby odeberou zastaralá zařízení. Toto nastavení je široké pro celou organizaci a po aktivaci vstoupí v platnost okamžitě. Všechna zařízení, která nejsou na serveru Intune po dobu přesahující toto nastavení, se trvale odstraní.

**Poznámka:** Pro tuto akci vyčištění jsou způsobilé pouze objekty zařízení MDM. EAS pouze objekty zařízení jsou vyloučeny.

Další informace o tom, kdy se zařízení stane způsobilým k odstranění na základě nastavení vyčištění zařízení a jeho "stavu":

Nastavení: **Odstranění zařízení po posledním datu vrácení se změnami: Ano (některé hodnoty (N) ve dnech zadaných)**

- Na základě hodnoty (N) nakonfigurované v nastavení služba Intune odstraní zařízení v určených dnech po posledním úspěšném vrácení se seznámí se se zpět.

Nastavení: **Odstranění zařízení po posledním datu vrácení se změnami: Ne**

- 180 dní po vypršení platnosti certifikátu zařízení a není obnoven, zařízení se odstraní.

**Poznámka:** V obou případech musí být zařízení úspěšně zaregistrováno v Intune. K registraci dojde během prvního vrácení se změnami zařízení se službou Intune.

Pokud se zařízení úspěšně zaregistruje do Intune, ale neasíduje intune, zařízení se odstraní 270 dní po registraci. (90 dní na označení zařízení jako odvolaného a dalších 180 dní na odstranění záznamu.)

V konzoli Intune momentálně neexistuje žádný mechanismus, který by stanovil datum vypršení platnosti certifikace zařízení pro dané zařízení.