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
# <a name="intune-exchange-on-premise-connector"></a>On-premises connector voor Exchange intune

Raadpleeg de volgende documentatie voor meer informatie over het instellen van een verbindingslijn tussen intune en Exchange die on-premises wordt gehost.

[De on-premises Exchange-connector van intune instellen in Microsoft intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**FAQ:**

V: Ik zie een foutbericht, bijvoorbeeld ' de versie van Exchange connector wordt niet ondersteund ' wordt weergegeven wanneer u probeert de Exchange connector in te stellen. Wat kan de oorzaak zijn?

A: het account dat u gebruikt, heeft een licentie voor u nodig-het moet een actieve intune-licentie hebben

V: is het mogelijk om meerdere Exchange-connectors te hebben?

A: u kunt maar één Exchange-connector per Exchange-organisatie instellen per intune-Tenant. De connector kan alleen worden geïnstalleerd op één server in een Exchange-organisatie met meerdere servers.

Daarnaast zijn er geen connectors geconfigureerd voor Exchange on-premises en Exchange Online geconfigureerd in dezelfde Tenant.

V: kan de connector een CAS-matrix als verbinding met Exchange maken?

A: als u een CAS-matrix opgeeft, is geen ondersteunde configuratie in de connectorconfiguratie. U moet slechts één server opgeven en moet een hardcoded-configuratiebestand zijn dat kan worden gevonden in

programma Data\Microsoft\Microsoft intune on-premises Exchange connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

Zoek de volgende vermelding ```<ExchangeWebServiceURL />``` en vervang de URL door de Exchange-Server.

**Voorbeeld**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Raadpleeg de volgende documentatie voor verdere probleemoplossing: [problemen met de on-premises Exchange-connector van intune oplossen](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Uitgebreide logboekregistratie inschakelen voor de Exchange connector**

1. Het configuratiebestand voor Exchange connector tracering openen voor bewerking.  
Het bestand bevindt zich op:%ProgramData%\Microsoft\Windows intune Exchange Connector\TracingConfiguration.xml  

**Voorbeeld**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Zoek de TraceSourceLine met de volgende sleutel: OnPremisesExchangeConnectorService  
  
3. Wijzig de waarde van het knooppunt SourceLevel van Information ActivityTracing (de standaardinstelling) in uitgebreide ActivityTracing  

**Voorbeeld**
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
4. De Microsoft intune Exchange-service opnieuw starten  
5. Volledige synchronisatie in de intune-Portal totdat deze is voltooid en wijzig vervolgens de XML weer in ' Information ActivityTracing ' en start de Microsoft intune Exchange-service opnieuw.  
6. Locatie van de logboeken is: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`