---
title: Automatické vyčištění zastaralých zařízení v Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715014"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatické vyčištění zastaralých zařízení v Intune

Intune umožňuje správci nakonfigurovat časový interval mezi 90 a 270 dny, po kterém se zastaralá zařízení odeberou ze služby. Toto nastavení je celé v organizaci a jakmile se aktivuje okamžitě. Všechna zařízení, která nejsou vrácená do serveru Intune po dobu, po kterou se nastavení trvale odstraní.

**Poznámka:** Pro tuto akci čištění jsou způsobilé pouze objekty zařízení MDM. Pouze objekty zařízení EAS jsou vyloučeny.

Další informace o tom, kdy se zařízení stane opravňujícím k odstranění na základě nastavení čištění zařízení a jeho stavu:

Nastavení: **odstranění zařízení po posledním vrácení se změnami: Ano (určitá hodnota (N) v zadaných dnech)**

- V závislosti na hodnotě (N), která je v nastavení nakonfigurovaná, služba Intune odstraní zařízení v zadaných dnech od posledního úspěšného ověření.

Nastavení:  **odstranění zařízení po posledním vrácení se změnami: ne**

- 180 dnů po vypršení platnosti certifikátu zařízení se odstraní.

**Poznámka:** V obou případech je nutné zařízení úspěšně zaregistrovat v Intune. Registrace proběhne v průběhu prvního vrácení se změnami zařízení se službou Intune.

Pokud se zařízení úspěšně zaregistruje do Intune, ale nezobrazuje se jako registrace, odstraní se zařízení 270 dní po zápisu. (90 dnů pro označení zařízení jako odvolaného a další 180 dní, než se záznam odstraní.)

V konzole Intune momentálně neexistuje žádný mechanismus pro určení data vypršení platnosti certifikace zařízení pro dané zařízení.