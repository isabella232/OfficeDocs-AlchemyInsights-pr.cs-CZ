---
title: soubory s postupy pro import –
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780052"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="9e9b8-102">Jak importovat soubory. NK2</span><span class="sxs-lookup"><span data-stu-id="9e9b8-102">How to import .nk2 files</span></span> 

<span data-ttu-id="9e9b8-103">Při prvním spuštění Microsoft Outlooku 2013, Outlooku 2016, Outlooku 2019 nebo Outlooku for Microsoft 365 se vaše mezipaměť přezdívky (uložená v souboru *Profile*. NK2) naimportuje do skryté zprávy ve svém výchozím úložišti zpráv.</span><span class="sxs-lookup"><span data-stu-id="9e9b8-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="9e9b8-104">Pokud chcete importovat soubory. NK2 do Outlook 2013, Outlooku 2016, Outlooku 2019 nebo Outlooku for Microsoft 365, zkontrolujte, jestli je soubor. NK2 v této složce:%appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="9e9b8-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="9e9b8-105">**Poznámka**: soubor. NK2 musí mít stejný název jako váš aktuální profil Outlook 2013 nebo Outlook 2016.</span><span class="sxs-lookup"><span data-stu-id="9e9b8-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="9e9b8-106">Ve výchozím nastavení je název profilu "Outlook".</span><span class="sxs-lookup"><span data-stu-id="9e9b8-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="9e9b8-107">Chcete-li zkontrolovat název profilu, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="9e9b8-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="9e9b8-108">Klepněte na tlačítko **Start** a poté na **Ovládací panely**.</span><span class="sxs-lookup"><span data-stu-id="9e9b8-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="9e9b8-109">Poklikejte na položku **Pošta**.</span><span class="sxs-lookup"><span data-stu-id="9e9b8-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="9e9b8-110">V dialogovém okně Nastavení pošty vyberte **Zobrazit profily**.</span><span class="sxs-lookup"><span data-stu-id="9e9b8-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="9e9b8-111">Vyberte **Spustit**  >  **spuštění**.</span><span class="sxs-lookup"><span data-stu-id="9e9b8-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="9e9b8-112">Do pole **otevřít** zadejte *outlook.exe/importnk2*a pak vyberte **OK**.</span><span class="sxs-lookup"><span data-stu-id="9e9b8-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="9e9b8-113">Po importu souboru. NK2 se obsah souboru sloučí do existující mezipaměti přezdívek, která je uložená ve vaší poštovní schránce.</span><span class="sxs-lookup"><span data-stu-id="9e9b8-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="9e9b8-114">**Poznámka**: při příštím spuštění outlooku 2013, outlooku 2016, outlooku 2019 nebo Outlooku for Microsoft 365 se soubor. NK2 přejmenuje o příponu. old.</span><span class="sxs-lookup"><span data-stu-id="9e9b8-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="9e9b8-115">Pokud chcete soubor. NK2 znovu importovat, odeberte nejprve příponu. old.</span><span class="sxs-lookup"><span data-stu-id="9e9b8-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="9e9b8-116">Další informace najdete v článku [Import nebo zkopírování seznamu automatického dokončování do jiného počítače](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span><span class="sxs-lookup"><span data-stu-id="9e9b8-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>