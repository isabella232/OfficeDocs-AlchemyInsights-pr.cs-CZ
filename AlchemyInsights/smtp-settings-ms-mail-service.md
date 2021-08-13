---
title: Nastavení SMTP pro Microsoft 365 poštovní službu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 373042e9593faf4eaa486313763beb8e8f48b6e9ea159d1cfb37b9df826384f4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813967"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>Nastavení SMTP pro Microsoft 365 poštovní službu

Toto jsou nastavení SMTP pro poštovní Microsoft 365 služby:

**Server:** smtp.office365.com </br>
**Port:** 587 </br>
**Šifrování:** STARTTLS (teď je podporovaná jenom verze TLS 1.2. Ujistěte se prosím, že vaše aplikace nebo zařízení podporují protokol TLS 1.2) </br>
**Uživatelské** jméno: Office 365 adresa (například example@yourdomain.com) </br>
**Heslo:** Vaše Office 365 heslo </br>
**Ověřování:** Povinné </br>
**Limity odesílání:** 10 000 e-mailů denně </br>

Informace o nastavení protokolu POP a IMAP najdete v tématu [Nastavení protokolu POP, IMAP a SMTP](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
Informace o možnostech předávání e-mailů pomocí Microsoft 365 a postupu najdete v tématu Nastavení multifunkčního zařízení nebo aplikace pro posílání e-mailů pomocí Microsoft 365 nebo [Office 365](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).