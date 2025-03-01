---
title: IP-adres en client identificeren in auditlogboeken
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 57a1756787f8297a2a1ab3012b95aaa2f33e6045
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313014"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-adres en client identificeren in auditlogboeken

Het IP-adres dat overeenkomt met een activiteit van een Microsoft 365 gebruiker of beheerder wordt weergegeven in de auditlogboeken. De clientgegevens worden ook vastgelegd. Hier volgen de stappen voor het identificeren van dergelijke informatie

1. Meld u aan bij [het Microsoft 365 compliancecentrum.](https://protection.office.com/)

2. Ga naar de **zoekpagina**  >  **Van het zoeklogboek zoeken.**

   Als u geïnteresseerd bent in een specifieke activiteit, selecteert u deze in **de lijst** Activiteiten. Als dit niet het beste is, worden alle activiteiten geretourneerd voor de geselecteerde gebruiker (standaardinstelling).

   **Opmerking:** Bepaalde activiteiten zijn mogelijk niet beschikbaar in **het** menu Activiteiten; Deze audititems worden echter geretourneerd als **Resultaten voor** alle activiteiten tonen is geselecteerd (standaardinstelling).

3. Geef de gebruikersnaam op in **het veld Gebruikers,** selecteer het juiste datumbereik voor de activiteit en klik vervolgens op **Zoeken**.

In de resultaten ziet u het IP-adres voor die activiteit in het resultatenvenster. Selecteer de auditrecord voor gedetailleerde informatie in de flyout **Details** (bijvoorbeeld Client, Gebruiker die actie heeft uitgevoerd, enzovoort).

Zie Het IP-adres zoeken van de computer die wordt gebruikt voor toegang tot [een gekromd account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)voor meer informatie.
