---
title: Řešení chyb při ověřování toku
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3c4ad806ed446803d8c1e0ba17b3a06d591985d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690560"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="27d0a-102">Řešení chyb při ověřování toku</span><span class="sxs-lookup"><span data-stu-id="27d0a-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="27d0a-103">V mnoha případech se chyby nedaří kvůli chybě ověřování.</span><span class="sxs-lookup"><span data-stu-id="27d0a-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="27d0a-104">Pokud máte tento typ chyby, chybová zpráva obsahuje "Neautorizováno" nebo se zobrazí kód chyby 401 nebo 403.</span><span class="sxs-lookup"><span data-stu-id="27d0a-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="27d0a-105">Chybu ověřování obvykle opravíte aktualizací připojení:</span><span class="sxs-lookup"><span data-stu-id="27d0a-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="27d0a-106">V horní části webového portálu klikněte nebo klepněte na ikonu ozubeného kola a otevřete nabídku nastavení a pak klikněte nebo klepněte na **připojení**.</span><span class="sxs-lookup"><span data-stu-id="27d0a-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="27d0a-107">Přejděte na připojení, u kterého se zobrazila chybová zpráva o neoprávněné chybě.</span><span class="sxs-lookup"><span data-stu-id="27d0a-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="27d0a-108">Vedle připojení klikněte nebo klepněte na odkaz **ověřit heslo** ve zprávě o připojení, které se neověřuje.</span><span class="sxs-lookup"><span data-stu-id="27d0a-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="27d0a-109">Ověřte svoje přihlašovací údaje podle pokynů, které se zobrazí, vraťte se ke svému toku a potom klikněte nebo klepněte na **znovu odeslat**.</span><span class="sxs-lookup"><span data-stu-id="27d0a-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="27d0a-110">Další nápovědu najdete v tématu [Poradce při potížích s tokem toku](https://go.microsoft.com/fwlink/?linkid=872110).</span><span class="sxs-lookup"><span data-stu-id="27d0a-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

