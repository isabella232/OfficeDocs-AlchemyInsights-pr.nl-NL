---
title: On-premises connector voor Exchange intune
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
ms.contentlocale: nl-NL
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807398"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="445af-102">On-premises connector voor Exchange intune</span><span class="sxs-lookup"><span data-stu-id="445af-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="445af-103">Raadpleeg de volgende documentatie voor meer informatie over het instellen van een verbindingslijn tussen intune en Exchange die on-premises wordt gehost.</span><span class="sxs-lookup"><span data-stu-id="445af-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="445af-104">De on-premises Exchange-connector van intune instellen in Microsoft intune Azure</span><span class="sxs-lookup"><span data-stu-id="445af-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="445af-105">**FAQ:**</span><span class="sxs-lookup"><span data-stu-id="445af-105">**FAQ:**</span></span>

<span data-ttu-id="445af-106">V: Ik zie een foutbericht, bijvoorbeeld ' de versie van Exchange connector wordt niet ondersteund ' wordt weergegeven wanneer u probeert de Exchange connector in te stellen.</span><span class="sxs-lookup"><span data-stu-id="445af-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="445af-107">Wat kan de oorzaak zijn?</span><span class="sxs-lookup"><span data-stu-id="445af-107">What could be the cause?</span></span>

<span data-ttu-id="445af-108">A: het account dat u gebruikt, heeft een licentie voor u nodig-het moet een actieve intune-licentie hebben</span><span class="sxs-lookup"><span data-stu-id="445af-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="445af-109">V: is het mogelijk om meerdere Exchange-connectors te hebben?</span><span class="sxs-lookup"><span data-stu-id="445af-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="445af-110">A: u kunt maar één Exchange-connector per Exchange-organisatie instellen per intune-Tenant.</span><span class="sxs-lookup"><span data-stu-id="445af-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="445af-111">De connector kan alleen worden geïnstalleerd op één server in een Exchange-organisatie met meerdere servers.</span><span class="sxs-lookup"><span data-stu-id="445af-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="445af-112">Daarnaast zijn er geen connectors geconfigureerd voor Exchange on-premises en Exchange Online geconfigureerd in dezelfde Tenant.</span><span class="sxs-lookup"><span data-stu-id="445af-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="445af-113">V: kan de connector een CAS-matrix als verbinding met Exchange maken?</span><span class="sxs-lookup"><span data-stu-id="445af-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="445af-114">A: als u een CAS-matrix opgeeft, is geen ondersteunde configuratie in de connectorconfiguratie.</span><span class="sxs-lookup"><span data-stu-id="445af-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="445af-115">U moet slechts één server opgeven en moet een hardcoded-configuratiebestand zijn dat kan worden gevonden in</span><span class="sxs-lookup"><span data-stu-id="445af-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="445af-116">programma Data\Microsoft\Microsoft intune on-premises Exchange connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="445af-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="445af-117">Zoek de volgende vermelding ```<ExchangeWebServiceURL />``` en vervang de URL door de Exchange-Server.</span><span class="sxs-lookup"><span data-stu-id="445af-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="445af-118">**Voorbeeld**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="445af-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="445af-119">Raadpleeg de volgende documentatie voor verdere probleemoplossing: [problemen met de on-premises Exchange-connector van intune oplossen](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="445af-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="445af-120">**Uitgebreide logboekregistratie inschakelen voor de Exchange connector**</span><span class="sxs-lookup"><span data-stu-id="445af-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="445af-121">Het configuratiebestand voor Exchange connector tracering openen voor bewerking.</span><span class="sxs-lookup"><span data-stu-id="445af-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="445af-122">Het bestand bevindt zich op:%ProgramData%\Microsoft\Windows intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="445af-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="445af-123">**Voorbeeld**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="445af-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="445af-124">Zoek de TraceSourceLine met de volgende sleutel: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="445af-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="445af-125">Wijzig de waarde van het knooppunt SourceLevel van Information ActivityTracing (de standaardinstelling) in uitgebreide ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="445af-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="445af-126">**Voorbeeld**</span><span class="sxs-lookup"><span data-stu-id="445af-126">**Example:**</span></span>
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
4. <span data-ttu-id="445af-127">De Microsoft intune Exchange-service opnieuw starten</span><span class="sxs-lookup"><span data-stu-id="445af-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="445af-128">Volledige synchronisatie in de intune-Portal totdat deze is voltooid en wijzig vervolgens de XML weer in ' Information ActivityTracing ' en start de Microsoft intune Exchange-service opnieuw.</span><span class="sxs-lookup"><span data-stu-id="445af-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="445af-129">Locatie van de logboeken is: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="445af-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>