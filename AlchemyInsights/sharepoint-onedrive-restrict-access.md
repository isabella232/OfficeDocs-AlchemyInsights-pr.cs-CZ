---
title: Omezení přístupu v SharePoint nebo OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093812"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Omezení přístupu v SharePoint nebo OneDrive

Existuje mnoho způsobů, jak omezit přístup k SharePoint online/OneDrive služeb. Tyto různé metody omezení přístupu jsou uvedené níže. 

**Omezení oprávnění**

V SharePoint Online a OneDrive pro firmy omezujeme přístup k položkám, jako jsou weby, soubory a složky, tím, že udělíme přístup jenom těm skupinám nebo jednotlivcům, kteří by měli mít přístup.

- [Přizpůsobení oprávnění pro SharePoint seznamu nebo knihovny](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Přizpůsobení SharePoint webu](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Změna oprávnění u podsložky](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Řízení přístupu z nespravovaných zařízení](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Jako SharePoint nebo globální správce můžete blokovat nebo omezit přístup k obsahu SharePoint a OneDrive z nespravovaných zařízení (ty, které nejsou připojené k hybridní službě AD nebo nejsou kompatibilní s Intune).

**Omezení umístění v síti**

Jako správce IT můžete řídit přístup k SharePoint a OneDrive na základě definovaných síťových umístění, která důvěřujete. Tato zásada se taky označuje jako zásada založená na poloze. Další informace najdete v tématu Řízení přístupu k SharePoint Online a [OneDrive na základě umístění v síti.](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Omezení uzamčení webu** 

V SharePoint Online máte možnost kolekci webů zamknout, takže nikdo nemá přístup. Tato možnost se nastaví přes PowerShell a [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomocí vlastnosti [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Omezení vytváření webů nebo podřízených webů uživatelům**

Jako správce SharePoint nebo globální správce můžete uživatelům nechat vytvářet SharePoint spravovat vlastní weby SharePoint, určit, jaký druh webů může vytvořit, a určit umístění webů. Další informace najdete v tématu Správa vytváření [webů v SharePoint Online.](https://docs.microsoft.com/sharepoint/manage-site-creation)

