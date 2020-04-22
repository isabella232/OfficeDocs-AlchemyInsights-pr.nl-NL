---
title: IP-adres en client identificeren in controlelogboeken
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716383"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-adres en client identificeren in controlelogboeken

Het IP-adres dat overeenkomt met een activiteit van een Microsoft 365-gebruiker of -beheerder wordt weergegeven in de controlelogboeken. De klantinformatie wordt ook geregistreerd. Hier volgen de stappen om dergelijke informatie te identificeren

1. Meld u aan bij het [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Ga naar de**zoekpagina van het zoekcontrolelogboek.** **Search** > 

   Als u geïnteresseerd bent in een specifieke activiteit, selecteert u deze in de lijst **Activiteiten.** Als dit niet het zo is, worden alle activiteiten geretourneerd voor de geselecteerde gebruiker (standaardinstelling).

   **Opmerking**: bepaalde activiteiten zijn mogelijk niet beschikbaar in het **menu Activiteiten;** Deze controleitems worden echter geretourneerd als **Resultaten weergeven voor alle activiteiten** is geselecteerd (standaardinstelling).

3. Geef de gebruikersnaam op in het veld **Gebruikers,** selecteer het juiste datumbereik voor de activiteit en klik op **Zoeken**.

In de resultaten ziet u het IP-adres voor die activiteit in het resultatenvenster. Selecteer de controlerecord om gedetailleerde informatie te zien in de **flyout Details** (bijvoorbeeld Client, Gebruiker die actie heeft uitgevoerd, enz.).

Zie [Het IP-adres van de computer die wordt gebruikt om toegang te krijgen tot een gecompromitteerd account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)voor meer informatie .
