---
title: Omezení přístupu v SharePointu nebo OneDrivu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700448"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Omezení přístupu v SharePointu nebo OneDrivu

Existuje mnoho způsobů, jak omezit přístup ke službám SharePoint Online/OneDrive. Níže jsou uvedené různé metody omezení přístupu. 

**Omezení oprávnění**

V SharePointu Online a OneDrivu pro firmy omezujeme přístup k položkám, jako jsou weby, soubory a složky, udělením přístupu pouze k těmto skupinám nebo jednotlivcům, kteří by měli mít přístup.

- [Přizpůsobení oprávnění pro SharePointový seznam nebo knihovnu](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Přizpůsobení oprávnění SharePointového webu](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Změna oprávnění u podsložky](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Řízení přístupu z nespravovaných zařízení](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Jako SharePointový nebo globální správce můžete blokovat nebo omezit přístup k obsahu SharePointu a OneDrivu z nespravovaných zařízení (což není hybridní služba AD spojená nebo kompatibilní v Intune).

**Omezení síťového umístění**

Jako správce IT můžete řídit přístup k prostředkům SharePoint a OneDrive na základě definovaných síťových umístění, kterým důvěřujete. Toto se označuje také jako zásady založené na poloze. Další informace najdete v tématu [řízení přístupu k datům SharePointu Online a OneDrivu na základě síťového umístění](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) .

**Omezení uzamčení webu** 

V SharePointu Online můžete kolekci webů uzamknout, takže nikdo nemá přístup. To se nastavuje prostřednictvím PowerShellu a [prostředí SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomocí vlastnosti [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Zakázání vytváření webů a podřízených webů uživateli**

Jako správce SharePointu nebo globální správce můžete uživatelům dovolit vytvářet a spravovat vlastní weby služby SharePoint, určit, jaký typ webů můžou vytvářet, a určit umístění webů. Další informace najdete v tématu [Správa vytváření webů v SharePointu Online](https://docs.microsoft.com/sharepoint/manage-site-creation) .

