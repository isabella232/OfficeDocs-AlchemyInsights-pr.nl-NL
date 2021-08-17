---
title: Hebben jouw gebruikers een schadelijke e-mail ontvangen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 608e2226c055f58ecf4f62e3c913106a6d319190ed6b317508e41514c12ba5d0
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893398"
---
# <a name="did-your-users-receive-malicious-email"></a>Hebben jouw gebruikers een schadelijke e-mail ontvangen?

U kunt nu de schadelijke e-mail rapporteren aan Microsoft met [inzendingen in Microsoft 365 Defender portal.](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Berichten die worden verzonden in [beheerdersinzendingen,](https://security.microsoft.com/reportsubmission?viewid=admin) worden gescand en de volgende resultaten worden weergegeven in de detail flyout:

- Of er tijdens de levering een fout zat in de e-mailverificatie van de afzender.
- Informatie over eventuele beleidstreffers die het oordeel over een bericht kunnen hebben beïnvloed of overschreven.
- Huidige deactiveringsresultaten om te zien of de URL's of bestanden in het bericht schadelijk waren of niet.
- Feedback van beoordelaars

Als een overschrijving is gevonden, zou het opnieuw scannen in enkele minuten moeten zijn voltooid. Als er geen probleem met de e-mailverificatie was of de levering niet werd beïnvloed door een overschrijving, kan de feedback van beoordelaars maximaal een dag duren.

Als je het niet eens bent met het uiteindelijke oordeel over een bericht, URL of bestand (geblokkeerd of niet geblokkeerd), dien het bericht dan na een dag opnieuw in voor een nieuwe scan. De kans is groot dat het oordeel verandert nadat je het bericht opnieuw hebt ingediend.

Ondertussen kun je schadelijke e-mail verwijderen uit het postvak IN van gebruikers met behulp van de instructies in [dit artikel](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Klanten met Microsoft Defender voor Office 365 kunnen:
  - [Bedreigingsverkenner gebruiken om verdachte e-mail te zoeken en te verwijderen](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Gebruik Safe koppelingen om toegang tot een](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) schadelijke URL te blokkeren
  - Gebruikers bijhouden die op schadelijke URL's hebben geklikt en deze hebben bekeken: [Bekijk phishing-URL](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)en klik op vonnisgegevens  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Handmatig een [geautomatiseerd onderzoek starten](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Je kunt ook beveiligen tegen schadelijke bestanden en URL's door de instructies te volgen in [Beveiligen tegen schadelijke URL's en bestanden](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
