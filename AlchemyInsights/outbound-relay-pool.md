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
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381632"
---
# <a name="outbound-relay-pool"></a>Uitgaande relaygroep

Microsoft wijzigt de configuratie voor het doorsturen of doorsturen van e-mail via Microsoft 365. Berichten in bepaalde scenario's worden doorgestuurd of doorgestuurd via Microsoft 365 met een speciale relaygroep. Berichten die worden verzonden met behulp van de relaisgroep, kunnen in de map ongewenste e-mail van de geadresseerde komen te staan. Zie Uitgaande [bezorgingsgroepen voor meer informatie.](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Als u een scenario wilt vermijden met de relaygroep, moet u ervoor zorgen dat doorgestuurde/doorgestuurde berichten voldoen aan een van de volgende criteria:

- De uitgaande afzender is een geaccepteerd domein van de tenant.
- Sender Policy Framework (SPF) wordt pas weergegeven wanneer het bericht wordt Microsoft 365.
- DomainKeys Identified Mail (DKIM) op het domein van de P2-afzender wordt weergegeven wanneer het bericht wordt Microsoft 365.
 
Berichten die voldoen aan de bovenstaande criteria, worden niet door de relaygroep verzonden.

Als de MX-record voor uw domein is gericht op een externe of on-premises server, gebruikt u verbeterde filtering om ervoor te zorgen dat de SPF-validatie juist is voor binnenkomende e-mail en om te voorkomen dat e-mail wordt verzonden via de relaygroep.

**Hoe kunnen we zien of we worden beïnvloed door de relaisgroep?**

Als voor uw doorgestuurde of doorgestuurde e-mailberichten een van de bovenstaande criteria wordt gebruikt, worden berichten niet doorgestuurd via de doorgestuurde groep. Als een bericht echter via een relaygroep wordt verzonden, is het IP van de uitgaande server in het bereik 40.95.0.0/16 en bevat de naam van de uitgaande server **rly** in de naam.

