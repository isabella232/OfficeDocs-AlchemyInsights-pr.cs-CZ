---
title: Omezení přístupu v SharePoint nebo OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075033"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Omezení přístupu v SharePoint nebo OneDrive

V SharePoint a OneDrive omezte přístup k položkám, jako jsou soubory, složky a seznamy, tím, že udělíte přístup jenom skupinám nebo jednotlivcům, ke kterým chcete mít přístup. Ve výchozím nastavení jsou SharePoint oprávnění v hierarchii zděděna z vyšší úrovně. Soubor tedy dědí oprávnění ze složky, která dědí oprávnění z knihovny, která dědí oprávnění z webu.
  
Pokud nechcete sdílet všechny položky na webu, můžete sdílet na vyšší úrovni (například sdílením celého webu) a potom přerušit dědičnost. Nedoporučujeme to ale, protože v budoucnu je údržba oprávnění složitější a matoucí. Místo toho můžete udělat toto:
  
- Pokud například chcete sdílet veškerý obsah složky s výjimkou jednoho souboru v ní, přesuňte tento soubor do nového umístění, které není sdílené.
    
- Pokud máte ve složce dvě podsložky a chcete sdílet jednu podsložku se skupinami A a B a povolit přístup jenom skupině A k druhé podsložce, sdílejte nadřazenou složku se skupinou A a přidejte skupinu B do první podsložky.
    
[Ukončení sdílení souboru nebo složky ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

