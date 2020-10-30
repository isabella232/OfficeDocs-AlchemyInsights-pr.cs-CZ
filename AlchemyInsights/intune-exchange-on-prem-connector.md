---
title: Místní konektor Exchange Intune
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
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807399"
---
# <a name="intune-exchange-on-premise-connector"></a>Místní konektor Exchange Intune

Podrobné informace o tom, jak nastavit konektor mezi Intune a Exchange hostujícím místně, najdete v této dokumentaci:

[Nastavení Intune on-premised Exchange Connectoru v Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**ČAST**

Otázka: při pokusu o nastavení Exchange Connectoru se zobrazuje chybová zpráva, že se nepoužívá verze Exchange Connector. Jaká je příčina?

A: účet, který používáte, je odpovídajícím způsobem licencován

Otázka: je možné mít více konektorů Exchange?

A: můžete nastavit jenom jednu Exchange Connector pro tenanta Intune na organizaci Exchange. Konektor může být nainstalovaný jenom na jednom serveru v organizaci pro více serverů Exchange.

Také nemůžete mít nastavené konektory pro Exchange místně i Exchange Online nakonfigurované ve stejném tenantovi.

Otázka: pro připojení k Exchangi může konektor použít pole CAS?

A: zadání pole CAS není podporovanou konfigurací nastavení konektoru. Měl by být zadán jenom jeden server a měl by být hardcoded v konfiguračním souboru konektoru, který najdete v části

program data\microsoft\microsoft Intune na místní konektor Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml

Vyhledejte následující položku ```<ExchangeWebServiceURL />``` a nahraďte ji adresou URL serveru Exchange.

**Pøíklad**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Další řešení potíží najdete v následující dokumentaci: [Poradce při potížích s Intune místním Exchange konektorem](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Povolení podrobného protokolování konektoru Exchange**

1. Otevřete konfigurační soubor sledování konektoru Exchange Connector pro úpravy.  
Umístění souboru:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Pøíklad**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Vyhledejte TraceSourceLine pomocí následujícího klíče: OnPremisesExchangeConnectorService  
  
3. Změna hodnoty uzlu SourceLevel z informační ActivityTracing (výchozí) na Verbose ActivityTracing  

**Pøíklad**
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
4. Restartujte službu Microsoft Intune Exchange  
5. Úplnou synchronizaci na portálu Intune až do jeho dokončení a pak změňte zpátky XML na "informační ActivityTracing" a restartujte službu Microsoft Intune Exchange.  
6. Umístění protokolů je: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`