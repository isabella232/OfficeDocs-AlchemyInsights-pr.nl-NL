---
title: Hebben jouw gebruikers een schadelijke e-mail ontvangen
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291787"
---
# <a name="did-your-users-receive-malicious-email"></a>Hebben jouw gebruikers een schadelijke e-mail ontvangen?

- Je kunt de schadelijke e-mail nu rapporteren aan Microsoft via [Inzendingen van beheerder in het Beveiligings- en compliancecentrum](https://sip.protection.office.com/reportsubmission).

Berichten die zijn verzonden via [inzendingen van beheerder](https://sip.protection.office.com/reportsubmission) worden gescand en de volgende resultaten worden weergegeven in de **details**-flyout:

- Of er tijdens de levering een fout zat in de e-mailverificatie van de afzender.
- Informatie over eventuele beleidstreffers die het oordeel over een bericht kunnen hebben beïnvloed of overschreven.
- Huidige deactiveringsresultaten om te zien of de URL's of bestanden in het bericht schadelijk waren of niet.
- Feedback van beoordelaars

Als een overschrijving is gevonden, zou het opnieuw scannen in enkele minuten moeten zijn voltooid. Als er geen probleem met de e-mailverificatie was of de levering niet werd beïnvloed door een overschrijving, kan de feedback van beoordelaars maximaal een dag duren.

Als je het niet eens bent met het uiteindelijke oordeel over een bericht, URL of bestand (geblokkeerd of niet geblokkeerd), dien het bericht dan na een dag opnieuw in voor een nieuwe scan. De kans is groot dat het oordeel verandert nadat je het bericht opnieuw hebt ingediend.

Ondertussen kun je schadelijke e-mail verwijderen uit het postvak IN van gebruikers met behulp van de instructies in [dit artikel](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Klanten met Microsoft Defender voor Office 365 kunnen:
    - de [Bedreigingsverkenner gebruiken om verdachte e-mails te zoeken en te verwijderen](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [Veilige koppelingen gebruiken om de toegang tot een schadelijke URL te blokkeren](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)
    - gebruikers volgen die op schadelijke URL's hebben geklikt en deze hebben geopend: [bekijk de phishing-URL en klik op oordeelgegevens](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - handmatig [een geautomatiseerd onderzoek starten](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Je kunt ook beveiligen tegen schadelijke bestanden en URL's door de instructies te volgen in [Beveiligen tegen schadelijke URL's en bestanden](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).