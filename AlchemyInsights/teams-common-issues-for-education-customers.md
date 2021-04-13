---
title: Běžné problémy v Teams pro zákazníky verze Education
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 893c8cacaf089932014ba7a3ea6122d17da38cdd
ms.sourcegitcommit: ef7ec42aba3c06aa8966dfac71cec18c08e7acf8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/13/2021
ms.locfileid: "51692387"
---
# <a name="teams-common-issues-for-education-customers"></a>Běžné problémy v Teams pro zákazníky verze Education

**Pro zákazníky verze Education:**

Pokud potřebujete pomoct s nasazením Teams na podporu výuky na dálku, odešlete nám žádost prostřednictvím [centra FastTrack](https://www.microsoft.com/fasttrack). Projděte si následující běžné problémy, s kterými se potýkají zákazníci používající Teams ve verzi Education:

- Zobrazuje se vám zpráva **„Nevíte, o co přicházíte!“**? Nezapomeňte [povolit Microsoft Teams pro vaši školu](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). V tenantech EDU není služba Microsoft Teams ve výchozím nastavení povolená. Nejdřív ji budete muset zapnout.

- **Používáte Teams nově?** Přečtěte si téma [Vzdálená výuka a učení v Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4), kde jsou nejaktuálnější informace o nastavení vaší školy, plánování hodin, virtuálních schůzkách a sdílení obsahu se studenty.

- Jakmile je služba Teams povolena, můžou ji uživatelé spustit. Musí si k tomu nainstalovat [desktopového](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) nebo [mobilního](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients) klienta, případně použít verzi v prohlížeči na adrese https://teams.microsoft.com.

- **Povolení přístupu hostů do Teams:** Přečtěte si téma obsahující [kontrolní seznam pro přístup hostů do Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist) a splňte všechny uvedené kroky.
    - [Principy přístupu hostů v Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Nastavení – kontrolní seznam pro přístup hostů do Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Jak se host připojí k týmu](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Schůzky Teams a vytáčené připojení:** Potřebujete pomoct se zapnutím nebo nastavením audiokonferencí v Microsoft Teams? Byl tento uživatel nedávno vytvořen? Pokud ano, budete muset počkat 2 až 24 hodin, než se nastavení projeví. Abyste ověřili, jestli má uživatel licenci pro audiokonference a má výchozí číslo placené linky, udělejte tohle:
    1. Přejděte do seznamu Aktivní uživatelé a vyberte daného uživatele.
    2. V závislosti na verzi centra pro správu vyberte buď **Licence a aplikace**, nebo klikněte na možnost **Upravit** v záložce **Licence na produkty**.
    3. Potvrďte, že má uživatel vybrané licence pro Audiokonference, Microsoft Teams a Online Skype pro firmy (Plán 2).
    4. V centru pro správu uživatele klikněte na **Zobrazit vše** a pak na **Teams**.
    5. V centru pro správu Microsoft Teams klikněte na **Starší verze portálu**.
    6. V centru pro správu Skypu pro firmy klikněte na **Audiokonference** a pak na **Uživatelé**.
    7. Vyberte požadovaného uživatele a zkontrolujte, jestli má výchozí číslo placené linky.

    Další informace najdete v tématu [Plány](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) volání do Microsoft Teams nebo zavolejte týmu fakturace Microsoft Commerce, který vám pomůže s otázkami souvisejícími s licencování.

    Další zdroje informací

    - [Schůzky a konference v Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Audiokonference](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Zásady schůzek:** Zásady schůzek slouží k řízení funkcí, které jsou dostupné účastníkům schůzek naplánovaných uživateli ve vaší organizaci. Jakmile vytvoříte zásady a provedete požadované změny, můžete k zásadám přiřadit uživatele.

    - **Změna nebo vytvoření zásad schůzky:** Pokud chcete změnit nebo vytvořit zásady schůzky, přejděte do **Centra pro správu Microsoft Teams > Schůzky > Zásady schůzek**. Ze seznamu vyberte zásady nebo klikněte na **Přidat**. Jestliže vytváříte nové zásady, pojmenujte je a přidejte popis. Název nesmí obsahovat speciální znaky ani mít víc než 64 znaků. Zvolte požadovaná nastavení a potom klikněte na **Uložit**. 
    
        Řekněme třeba, že máte skupinku uživatelů a chcete omezit šířku pásma, kterou bude jejich schůzka vyžadovat. Vytvoříte nové vlastní zásady nazvané Omezená šířka pásma a zakážete následující nastavení:

        V části **Zvuk a video**:
        - Vypnete možnost **Povolit nahrávání do cloudu**.
        - Vypnete možnost **Povolit IP video**.

        V části **Sdílení obsahu**:

        - Zakážete režim sdílení obrazovky.
        - Vypnete možnost **Povolit tabuli**.
        - Vypnete možnost **Povolit sdílené poznámky**.

        Pak **zásady přiřadíte uživatelům**:

    1. V levém navigačním panelu centra pro správu Microsoft Teams přejděte na **Uživatelé** a klikněte na daného uživatele.
    2. Vyberte uživatele kliknutím vlevo od uživatelského jména a pak klikněte na **Upravit nastavení**.
    3. V části **Zásady schůzek** vyberte zásady, které chcete přiřadit, a klikněte na **Použít**.

    Pokud chcete přiřadit zásady více uživatelům současně, přečtěte si téma o [hromadné úpravě nastavení uživatelů Teams](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk).

    Nebo můžete postupovat takto:
    1. V levém navigačním panelu centra pro správu Microsoft Teams přejděte na **Schůzky > Zásady schůzek**.
    2. Kliknutím vlevo od názvu vyberte zásady.
    3. Klikněte na **Spravovat uživatele**.
    4. V podokně **Spravovat uživatele** vyhledejte uživatele podle zobrazovaného nebo uživatelského jména, vyberte ho a klikněte na **Přidat**. Tento krok opakujte pro všechny uživatele, které chcete přidat.
    5. Až přidávání uživatelů dokončíte, klikněte na **Uložit**.

- **Poradce při potížích s chybějícím číselníkem:**
    - Zkontrolujte, že má uživatel přiřazenou [licenci Teams](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses).
    - Zkontrolujte, že má uživatel přiřazený [volací plán](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page).
    - Povolte uživatelům [Enterprise Voice](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Poradce při potížích s přihlášením k Teams:** nejdřív zkontrolujte, jestli je [služba Microsoft Teams v pořádku](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Pak se podívejte na běžné kódy chyb a přečtěte si téma: [Proč se mi nedaří přihlásit se do Microsoft Teams?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f) Možná si také budete muset přečíst téma o [modelech identit a ověřování v Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).
