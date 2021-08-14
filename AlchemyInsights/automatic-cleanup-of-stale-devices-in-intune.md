---
title: Automatické čištění zastaralých zařízení v Intune
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
ms.openlocfilehash: 905881f08ace7afae871ac48fa30ed1a0f15d13972cdff299a6694ca2eafc9cc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53997057"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatické čištění zastaralých zařízení v Intune

Intune umožňuje správci nakonfigurovat časový interval mezi 90 a 270 dny, po kterém se ze služby odebrala zastaralá zařízení. Toto nastavení je pro celou organizaci a jakmile je aktivované, okamžitě se projeví. Všechna zařízení, která nejsou na serveru Intune zaškrtnutá po dobu přesahující toto nastavení, se trvale odstraní.

**Poznámka:** Pro tuto akci čištění mají nárok jenom objekty zařízení MDM. Objekty zařízení EAS jsou vyloučené.

Další informace o tom, kdy má zařízení nárok na odstranění na základě nastavení čištění zařízení a jeho stavu:

Nastavení: Odstranění zařízení po datu posledního **check-inu: Ano (některá hodnota (N) v zadaných dnech)**

- Na základě hodnoty (N) nakonfigurované v nastavení odstraní služba Intune zařízení v určených dnech po jeho posledním úspěšném vrácení se službou.

Nastavení:  **Odstranění zařízení po posledním datu rezervace: Ne**

- 180 dní po vypršení platnosti certifikátu zařízení a jeho prodloužení se zařízení odstraní.

**Poznámka:** V obou případech musí být zařízení úspěšně zaregistrované v Intune. Registrace probíhá během prvního přihlášení zařízení ke službě Intune.

Pokud se zařízení úspěšně zaregistruje do Intune, ale neregistruje se, zařízení se odstraní 270 dní po registraci. (90 dní k označení zařízení jako zrušené a pak dalších 180 dnů k odstranění záznamu.)

V konzole Intune v současné době neexistuje žádný mechanismus, který by pro dané zařízení vytvořil datum vypršení platnosti certifikace zařízení.