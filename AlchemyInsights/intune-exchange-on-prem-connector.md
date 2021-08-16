---
title: Intune Exchange on-premises Connector
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
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013959"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange on-premises Connector

Zie de volgende documentatie voor meer informatie over het instellen van de verbindingslijn tussen Intune en Exchange die on-premises wordt gehost:

[De on-premises Intune-verbindingslijn Exchange instellen in Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**FAQ:**

V: Ik zie een foutmelding zoals 'De Exchange Connector-versie wordt niet ondersteund' bij het instellen van de verbindingslijn Exchange connector. Wat kan de oorzaak zijn?

A: Het account dat u gebruikt, is op de juiste manier gelicentieerd: het moet een actieve Intune-licentie hebben

V: Is het mogelijk om meerdere verbindingslijnen Exchange gebruiken?

A: U kunt slechts één verbindingslijn Exchange Intune-tenant per organisatie Exchange instellen. De verbindingslijn kan slechts op één server in een exchange-organisatie met meerdere servers worden geïnstalleerd.

U kunt ook geen connectors configureren voor zowel Exchange on-premises als Exchange Online geconfigureerd in dezelfde tenant.

V: Kan de verbindingslijn een CAS-matrix gebruiken als verbinding met Exchange?

A: Het opgeven van een CAS-matrix is geen ondersteunde configuratie in de connectorinstallatie. Er moet slechts één server worden opgegeven en moeten worden gecodeerd in het configuratiebestand van de connector, dat kan worden gevonden in

program data\microsoft\microsoft Intune on premises Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Zoek de volgende vermelding ```<ExchangeWebServiceURL />``` en vervang de URL door de Exchange-server.

**Voorbeeld:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Raadpleeg de volgende documentatie voor aanvullende probleemoplossing: Problemen met de [on-premises Intune-verbindingslijn Exchange oplossen](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Verbose-logboekregistratie voor de Exchange inschakelen**

1. Open het configuratiebestand Exchange connectortracing voor bewerken.  
Het bestand bevindt zich op : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Voorbeeld:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Zoek de TraceSourceLine met de volgende sleutel: OnPremisesExchangeConnectorService  
  
3. De waarde van het knooppunt SourceLevel wijzigen van Information ActivityTracing (de standaardwaarde) in Verbose ActivityTracing  

**Voorbeeld:**
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
4. De service Microsoft Intune Exchange opnieuw starten  
5. Volledige synchronisatie in Intune Portal totdat deze is klaar en wijzig de XML weer in 'Information ActivityTracing' en start de Microsoft Intune Exchange Service.  
6. De locatie van de logboeken is: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`