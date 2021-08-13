---
title: Řešení problémů s načítáním obrázků v Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 11315fd84f92251e435320f4550286fb2db4b0128f7ac85c0f79972e3f7fd203
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939228"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>Řešení problémů s načítáním obrázků v Yammer

Když v aplikaci Yammer nastanou problémy s fotkami a náhledy souborů, vyřešte je tak, že se poohlédněte, jestli k problému dochází u všech uživatelů, jestli k tomuto problému dochází na mobilních zařízeních a jestli je reprodukovatelný při nahrávání přílohy.  

**Problémy s fotkou profilu**  

Pokud se koncoví uživatelé Yammer prostřednictvím Microsoft 365, musí změnit svůj profil, včetně své profilové fotky. Pokud uživatelé nemají oprávnění provádět aktualizace profilu, může správce tuto aktualizaci pro uživatele provést. Další informace najdete v tématu Zobrazení a [aktualizace profilu v Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).

Informace o úpravách profilu, včetně profilových fotek, najdete v tématu Změna [Yammer profilu a nastavení](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851). 

Aktualizované profilové fotky se synchronizují jinak než atributy profilu. Uživatelé se musí přihlásit, aby zahájili synchronizaci své profilové fotky. Informace najdete v článku [Jsou obrázky profilů uživatelů aktualizované z Office 365 na Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).

Informace o životním cyklu uživatelů pro Yammer najdete v tématu Správa Yammer uživatelů v celém jejich životním [cyklu od Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).  

Podrobnosti o tom, jak funguje synchronizace profilový obrázek v Microsoft 365, najdete v tématu Informace o synchronizaci obrázků profilu [v Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).  

**Problémy s náhledy dokumentů a miniaturami obrázků**  

Když jsou soubory nebo obrázky publikovány do Yammer, náhledy se nemusí zobrazit, protože: 

- Soubor je poškozený a nelze ho zpracovat.
- Soubor nebyl nedávno nahrán do SharePoint Online nebo Yammer neplatná metadata z jiných důvodů.
- Adresy URL potřebné k načtení obrázků náhledu jsou zablokované.
- Náhled souboru uživatel před publikováním odebral.
- Problém se službou znemožňoval generování náhledu.

**Poznámka:** Náhledy odkazů a nahrávání souborů se můžou chovat jinak. Odkazy na soubory na internetu nebo odkazy, které vyžadují další ověřování, se nemusí zobrazit správně.

Další informace najdete v tématu Připojení souboru nebo obrázku k [Yammer zprávy.](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf) 