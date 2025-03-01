---
title: Uitgaande relaygroep
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326072"
---
# <a name="outbound-relay-pool"></a>Uitgaande relaygroep

Microsoft wijzigt de configuratie voor het doorsturen of doorsturen van e-mail via Microsoft 365. Berichten in bepaalde scenario's worden doorgestuurd of doorgestuurd via Microsoft 365 met een speciale relaygroep. Berichten die worden verzonden met behulp van de relaisgroep, kunnen in de map ongewenste e-mail van de geadresseerde komen te staan. Zie Uitgaande [bezorgingsgroepen voor meer informatie.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Als u een scenario wilt vermijden met de relaygroep, moet u ervoor zorgen dat doorgestuurde/doorgestuurde berichten voldoen aan een van de volgende criteria:

- De uitgaande afzender is een geaccepteerd domein van de tenant.
- Sender Policy Framework (SPF) wordt pas weergegeven wanneer het bericht wordt Microsoft 365.
- DomainKeys Identified Mail (DKIM) op het domein van de P2-afzender wordt weergegeven wanneer het bericht wordt Microsoft 365.
 
Berichten die voldoen aan de bovenstaande criteria, worden niet door de relaygroep verzonden.

Als de MX-record voor uw domein is gericht op een externe of on-premises server, gebruikt u verbeterde filtering om ervoor te zorgen dat de SPF-validatie juist is voor binnenkomende e-mail en om te voorkomen dat e-mail wordt verzonden via de relaygroep.

**Hoe kunnen we zien of de relaisgroep ons beïnvloedt?**

Als voor uw doorgestuurde of doorgestuurde e-mailberichten een van de bovenstaande criteria wordt gebruikt, worden berichten niet doorgestuurd via de doorgestuurde groep. Als een bericht echter via een relaygroep wordt verzonden, is het IP van de uitgaande server in het bereik 40.95.0.0/16 en bevat de naam van de uitgaande server **rly** in de naam.

