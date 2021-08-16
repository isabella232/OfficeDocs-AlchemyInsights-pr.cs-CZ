---
title: Oznámení na Yammeru
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
- "9002878"
- "5480"
ms.openlocfilehash: a07d5f502beb61ab130e801b0e42579718f4d175a937fee4e21ab9f7339dbffd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097191"
---
# <a name="notifications-in-yammer"></a>Oznámení na Yammeru

Aby vás upozornil na novou aktivitu v relevantních konverzacích, [posílá Yammer oznámení](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) buď e-mailem, nebo když používáte Yammer na mobilním zařízení, prostřednictvím nabízených oznámení. Ve výchozím nastavení vám Yammer pošle upozornění na různé typy aktivit ve vaší síti. Uživatelé můžou aktualizovat nastavení e-mailu prostřednictvím webu Yammeru. Nabízená oznámení se nakonfigurují pomocí mobilní aplikace. 

Yammer přidal podporu [interaktivních e-mailů v Outlooku](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Některé e-maily (kopie zprávy) se stanou v Outlooku na webu interaktivními. Příští aktualizace tuto funkci přinese i do ostatních verzí Outlooku.

**Typy oznámení na Yammeru**

- E-maily (aktualizace ze skupiny, někdo vás zve do skupiny, přijde vám zpráva do složky doručené pošty atd.)
- Nabízená oznámení (posílaná na mobilních zařízeních, když vás někdo zmíní, přijde vám zpráva do složky doručené pošty atd.)
- Místní nabídky plochy (Když máte nainstalovanou desktopovou aplikaci Yammer, zobrazí se oznámení ve formě informační zprávy.)
- Upozornění zvonku (Na webu Yammeru se uživatelům zobrazí oznámení pro různé události. Tato oznámení nemusí mít vždycky přiřazený e-mail ani nabízené oznámení.)

K dispozici jsou další [podrobné informace o oznámeních](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Správa oznámení**

Uživatelé musí spravovat vlastní oznámení. Informace jsou k dispozici v tématu s popisem [povolení nebo zakázání e-mailových a mobilních oznámení Yammeru](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Správci nemůžou zakázat všechna oznámení nebo ovládat oznámení za uživatele. Správci můžou [řídit logo, které je součástí e-mailů, a jestli musí uživatelé potvrdit zprávy](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) poslané e-mailem.

**E-mailová oznámení odesílaná mnoha uživatelům ve vaší organizaci**

V některých případech Yammer pošle jedno oznámení e-mailem a obdrží ho mnohem víc uživatelů ve vaší organizaci, než jsme očekávali. K tomu dojde, když se do Yammeru přidá distribuční seznam nebo jiný typ nekonkrétní e-mailové adresy. Yammer vůbec neví, jestli e-mailová adresa patří jednomu uživateli, nebo se jedná o e-mailovou adresu, která umožňuje doručování jednoho e-mailu mnoha příjemcům. Když dojde k tomuto problému, musíte podniknout kroky, kterými [pozastavíte (deaktivujete) nesprávného uživatele s danou e-mailovou adresou](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) v Yammeru. 

Abyste snížili možnost výskytu tohoto problému, měli byste provést:

1. [Vynucení identity Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) pro uživatele Yammeru.
2. Blokování externích odesílatelů, aby nemohli posílat e-maily do vaší organizace, nebo omezení počtu odesílatelů na seznam schválených.

Pokud k tomuto problému dojde:

1. Identifikujte příjemce e-mailu, který by měl odpovídat uživateli v Yammeru. Například all-in-sales@fabrikam.com je distribuční seznam pro všechny prodejce. Tento distribuční seznam by mělo jít identifikovat z e-mailu Yammeru přijatého uživateli.
2. Pokud chcete potlačit uživatele s e-mailovou adresou all-in-sales@fabrikam.com, [deaktivujte (pozastavte) funkci ve správci sítě](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users). Pozastavení jde zrušit, takže je bezpečnější než odstranění. Odstranění uživatele proběhne automaticky po 90 dnech.
3. Případně můžete taky projít [export uživatelů](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) a identifikovat e-mailové adresy, které nepatří jednotlivým uživatelům a měly by být pozastavené.
