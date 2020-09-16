---
title: 'Chyba: změny se nedají nahrát nebo stáhnout, protože vypršela platnost přihlašovacích údajů uložených v mezipaměti.'
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "3534"
- "9001489"
ms.openlocfilehash: 8105fa7b311bc932f95c8bff4d6b58ed9aabe74a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734472"
---
# <a name="error-we-cant-upload-or-download-your-changes-because-your-cached-credentials-have-expired"></a><span data-ttu-id="96a14-102">Chyba: změny se nedají nahrát nebo stáhnout, protože vypršela platnost přihlašovacích údajů uložených v mezipaměti.</span><span class="sxs-lookup"><span data-stu-id="96a14-102">Error: We can't upload or download your changes because your cached credentials have expired</span></span>

<span data-ttu-id="96a14-103">Pokud se při ukládání souborů do aplikace OneDrive zobrazí chybová zpráva s informacemi o tom, že **vypršela platnost přihlašovacích údajů uložených v mezipaměti**, udělejte tyto kroky:</span><span class="sxs-lookup"><span data-stu-id="96a14-103">When saving files to the OneDrive app, if you receive an error that contains the phrase **"your cached credentials have expired"**, perform the following steps:</span></span>

1. <span data-ttu-id="96a14-104">Zavřete všechny aplikace Office.</span><span class="sxs-lookup"><span data-stu-id="96a14-104">Close all Office applications.</span></span>
1. <span data-ttu-id="96a14-105">Otevřete Správce přihlašovacích údajů a do vyhledávacího pole na hlavním panelu zadejte **Správce přihlašovacích** údajů a pak vyberte **ovládací panel Správce přihlašovacích údajů**.</span><span class="sxs-lookup"><span data-stu-id="96a14-105">Open Credential Manager, and type **credential manager** in the search box on the taskbar, then select **Credential Manager Control panel**.</span></span>
1. <span data-ttu-id="96a14-106">Vyberte **přihlašovací údaje systému Windows**.</span><span class="sxs-lookup"><span data-stu-id="96a14-106">Select **Windows Credentials**.</span></span>
1. <span data-ttu-id="96a14-107">Najděte všechny položky, které začínají na **OneDrivu**.</span><span class="sxs-lookup"><span data-stu-id="96a14-107">Find any entry that starts with the word **OneDrive**.</span></span>
1. <span data-ttu-id="96a14-108">Vyberte položku a stiskněte klávesu **Remove**.</span><span class="sxs-lookup"><span data-stu-id="96a14-108">Select the entry, then press **Remove**.</span></span>
1. <span data-ttu-id="96a14-109">Zavřete Správce přihlašovacích údajů, pak klikněte pravým tlačítkem na modrý Cloud v povíracích a vyberte **Zavřít OneDrive**.</span><span class="sxs-lookup"><span data-stu-id="96a14-109">Close Credential Manager, then right click on the blue cloud in your systray, and select **Close OneDrive**.</span></span>
1. <span data-ttu-id="96a14-110">Do vyhledávacího pole na hlavním panelu zadejte **OneDrive** a vyberte **aplikace OneDrive** a spusťte OneDrive.</span><span class="sxs-lookup"><span data-stu-id="96a14-110">Type **OneDrive** into the search box on the taskbar and select **OneDrive App** to launch OneDrive.</span></span>
1. <span data-ttu-id="96a14-111">Přihlaste se k OneDrivu a zkuste soubor uložit na OneDrive.</span><span class="sxs-lookup"><span data-stu-id="96a14-111">Sign into OneDrive, then try to save the file to OneDrive.</span></span>
