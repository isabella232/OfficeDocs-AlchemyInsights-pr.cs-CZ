---
title: Řešení problémů s načítáním obrázku v Yammeru
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
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690236"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>Řešení problémů s načítáním obrázku v Yammeru

Když se v Yammeru vyskytnou problémy s náhledy fotek a souborů, zkuste problém vyřešit tak, že zkontrolujete, jestli k problému dochází u všech uživatelů, jestli k němu dojde na mobilních zařízeních, a jestli je při nahrání přílohy reprodukovatelná.  

**Problémy s fotkou profilu**  

Pokud se koncoví uživatelé přihlásí do služby Yammer přes Microsoft 365, musí změnit profil, včetně fotografie profilu. Pokud uživatelé nemají oprávnění k aktualizaci profilu, může správce tuto aktualizaci učinit. Další informace najdete v článku [zobrazení a aktualizace profilu v Office Delvu](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).

Informace o úpravách profilů, včetně fotografií profilu, najdete v tématu [Změna profilu a nastavení Yammeru](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851). 

Aktualizované fotografie profilu se synchronizují jinak než atributy profilu. Uživatelé se musí přihlásit, abyste mohli zahájit synchronizaci své fotky profilu. Informace najdete v tématu [obrázky profilů uživatelů aktualizované z Office 365 na Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).

Informace o životním cyklu uživatele pro Yammer najdete v tématu [Správa uživatelů Yammeru napříč životním cyklem z Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).  

Podrobnosti o tom, jak synchronizace obrázků v profilu funguje v Microsoft 365, najdete v tématu [informace o synchronizaci profilů obrázků v microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).  

**Problémy s náhledy dokumentů a miniaturami obrázků**  

Když se do Yammeru zaúčtují soubory nebo obrázky, nemusí se zobrazit náhledy z těchto důvodů: 

- Soubor je poškozený a nedá se zpracovat.
- Soubor nebyl nedávno nahrán v SharePointu Online nebo Yammer nemá platná metadata z jiných důvodů.
- Adresy URL potřebné k načtení obrázků náhledu jsou blokovány.
- Náhled souboru byl před odesláním odebrán uživatelem.
- Chyba služby zabránila vygenerování náhledu.

**Poznámka:** Náhledy odkazů a odesílání souborů se můžou chovat jinak. Odkazy na soubory na internetu nebo odkazy, které vyžadují další ověřování, se nemusí zobrazovat správně.

Další informace najdete v článku [připojení souboru nebo obrázku ke zprávě Yammeru](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf). 