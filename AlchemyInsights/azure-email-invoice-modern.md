---
title: Moderní e-mailová fakturace Azure
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
- "9003801"
- "6866"
ms.openlocfilehash: caf300873c3a9a97502819c7938ecc86491795d2fc7b6f022ead5d38ca965b8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082827"
---
# <a name="email-invoicing-in-azure"></a>E-mailová fakturace v Azure

Abyste mohli aktualizovat předvolby e-mailové fakturace, musíte mít na fakturačním profilu nebo na jeho fakturačním účtu roli vlastníka nebo přispěvatele. Jakmile to odsouhlasíte, všichni uživatelé s rolí vlastníka, přispěvatele, čtenáře a správce faktur na fakturačním profilu dostanou fakturu tohoto profilu e-mailem.

1. Přihlaste se na [portál Microsoft Azure](https://portal.azure.com/).
2. Vyhledejte položku **Správa nákladů + fakturace**.
3. Vyberte **Faktury** na levé straně a v horní části stránky pak vyberte možnost **Poslat fakturu e-mailem**.
4. Pokud máte fakturačních profilů víc, vyberte některý z nich a pak vyberte **Vyjádřit souhlas**.

5. Vyberte **Aktualizovat**.
6. Pokud máte fakturačních profilů víc, vyberte některý z nich a pak vyberte **Vyjádřit souhlas**.

Ostatním uživatelům můžete udělit přístup k zobrazování, stahování a placení faktur tím, že jim přiřadíte roli správce faktur pro fakturační profil MCA nebo MPA. Pokud jste odsouhlasili, že faktury budete dostávat e-mailem, i uživatelům budou chodit faktury e-mailem.

1. Přihlaste se na [portál Microsoft Azure](https://portal.azure.com/).
2. Vyhledejte položku **Správa nákladů + fakturace**.
3. Vyberte **Fakturační profily** na levé straně. V seznamu fakturačních profilů vyberte fakturační profil, ke kterému chcete přiřadit roli správce faktur.
4. Vyberte **Řízení přístupu (systém IAM)** na levé straně a pak vyberte **Přidat** v horní části stránky.

V rozevíracím seznamu Role vyberte **Správce faktur**. Zadejte e-mailovou adresu uživatele, kterému chcete udělit přístup. Výběrem možnosti **Uložit** roli přiřadíte.
