---
title: Intune Exchange místní konektor
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013957"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange místní konektor

Podrobnosti o nastavení konektoru mezi Intune a Exchange, který je hostovaný místně, najdete v následující dokumentaci:

[Nastavení místního konektoru Intune Exchange Azure Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Časté otázky:**

Otázka: Při pokusu o nastavení konektoru Exchange konektoru se zobrazí chybová zpráva Exchange konektoru aplikace Exchange Connector. Co může být příčinou?

A: Účet, který používáte, je licencován odpovídajícím způsobem – musí mít aktivní licenci Intune.

Otázka: Je možné mít více Exchange konektorů?

O: Pro jednoho tenanta Intune můžete nastavit jenom Exchange konektor pro každou Exchange intune. Konektor se instaluje jenom na jeden server v organizaci pro výměnu více serverů.

Také nemůžete mít nakonfigurované konektory pro místní Exchange i pro Exchange Online nakonfigurované ve stejném tenantovi.

Otázka: Může spojnice použít matici CAS jako své připojení k Exchange?

A: Zadání matice CAS není podporovaná konfigurace v nastavení spojnice. Měl by být určen jenom jeden server a měl by být pevně zakódovaný v konfiguračním souboru konektoru, který najdete v

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Vyhledejte následující položku ```<ExchangeWebServiceURL />``` a nahraďte adresu URL exchange serverem.

**Příklad:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Další řešení potíží najdete v následující dokumentaci: Řešení potíží s místním [konektorem Exchange Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Povolení podrobného protokolování pro Exchange konektor**

1. Otevřete konfigurační soubor Exchange konektoru pro úpravy.  
Soubor se nachází na adrese : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Příklad:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Vyhledejte tracesourceline s následujícím klíčem: OnPremisesExchangeConnectorService  
  
3. Změna hodnoty uzlu SourceLevel z informace ActivityTracing (výchozí) na Verbose ActivityTracing  

**Příklad:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Restartujte službu Microsoft Intune Exchange.  
5. Úplná synchronizace na portálu Intune, dokud se nedokončí, a potom změňte xml zpět na "Information ActivityTracing" (Informační aktivita) a restartujte Microsoft Intune Exchange service.  
6. Umístění protokolů je: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`