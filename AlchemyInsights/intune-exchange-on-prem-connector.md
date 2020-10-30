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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="bba77-102">Místní konektor Exchange Intune</span><span class="sxs-lookup"><span data-stu-id="bba77-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="bba77-103">Podrobné informace o tom, jak nastavit konektor mezi Intune a Exchange hostujícím místně, najdete v této dokumentaci:</span><span class="sxs-lookup"><span data-stu-id="bba77-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="bba77-104">Nastavení Intune on-premised Exchange Connectoru v Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="bba77-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="bba77-105">**ČAST**</span><span class="sxs-lookup"><span data-stu-id="bba77-105">**FAQ:**</span></span>

<span data-ttu-id="bba77-106">Otázka: při pokusu o nastavení Exchange Connectoru se zobrazuje chybová zpráva, že se nepoužívá verze Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="bba77-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="bba77-107">Jaká je příčina?</span><span class="sxs-lookup"><span data-stu-id="bba77-107">What could be the cause?</span></span>

<span data-ttu-id="bba77-108">A: účet, který používáte, je odpovídajícím způsobem licencován</span><span class="sxs-lookup"><span data-stu-id="bba77-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="bba77-109">Otázka: je možné mít více konektorů Exchange?</span><span class="sxs-lookup"><span data-stu-id="bba77-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="bba77-110">A: můžete nastavit jenom jednu Exchange Connector pro tenanta Intune na organizaci Exchange.</span><span class="sxs-lookup"><span data-stu-id="bba77-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="bba77-111">Konektor může být nainstalovaný jenom na jednom serveru v organizaci pro více serverů Exchange.</span><span class="sxs-lookup"><span data-stu-id="bba77-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="bba77-112">Také nemůžete mít nastavené konektory pro Exchange místně i Exchange Online nakonfigurované ve stejném tenantovi.</span><span class="sxs-lookup"><span data-stu-id="bba77-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="bba77-113">Otázka: pro připojení k Exchangi může konektor použít pole CAS?</span><span class="sxs-lookup"><span data-stu-id="bba77-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="bba77-114">A: zadání pole CAS není podporovanou konfigurací nastavení konektoru.</span><span class="sxs-lookup"><span data-stu-id="bba77-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="bba77-115">Měl by být zadán jenom jeden server a měl by být hardcoded v konfiguračním souboru konektoru, který najdete v části</span><span class="sxs-lookup"><span data-stu-id="bba77-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="bba77-116">program data\microsoft\microsoft Intune na místní konektor Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="bba77-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="bba77-117">Vyhledejte následující položku ```<ExchangeWebServiceURL />``` a nahraďte ji adresou URL serveru Exchange.</span><span class="sxs-lookup"><span data-stu-id="bba77-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="bba77-118">**Pøíklad**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="bba77-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="bba77-119">Další řešení potíží najdete v následující dokumentaci: [Poradce při potížích s Intune místním Exchange konektorem](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="bba77-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="bba77-120">**Povolení podrobného protokolování konektoru Exchange**</span><span class="sxs-lookup"><span data-stu-id="bba77-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="bba77-121">Otevřete konfigurační soubor sledování konektoru Exchange Connector pro úpravy.</span><span class="sxs-lookup"><span data-stu-id="bba77-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="bba77-122">Umístění souboru:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="bba77-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="bba77-123">**Pøíklad**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="bba77-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="bba77-124">Vyhledejte TraceSourceLine pomocí následujícího klíče: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="bba77-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="bba77-125">Změna hodnoty uzlu SourceLevel z informační ActivityTracing (výchozí) na Verbose ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="bba77-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="bba77-126">**Pøíklad**</span><span class="sxs-lookup"><span data-stu-id="bba77-126">**Example:**</span></span>
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
4. <span data-ttu-id="bba77-127">Restartujte službu Microsoft Intune Exchange</span><span class="sxs-lookup"><span data-stu-id="bba77-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="bba77-128">Úplnou synchronizaci na portálu Intune až do jeho dokončení a pak změňte zpátky XML na "informační ActivityTracing" a restartujte službu Microsoft Intune Exchange.</span><span class="sxs-lookup"><span data-stu-id="bba77-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="bba77-129">Umístění protokolů je: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="bba77-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>