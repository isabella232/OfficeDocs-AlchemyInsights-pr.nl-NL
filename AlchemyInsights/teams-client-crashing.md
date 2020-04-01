---
title: Teams-cliënt crasht?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030588"
---
# <a name="teams-client-crashing"></a>Teams-cliënt crasht?

Als uw Teams-client crasht, probeer dan het volgende:

- Als u de Teams-desktop-app gebruikt, [ zorg dan dat de app volledig is bijgewerkt ](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Zorg ervoor dat alle [ URL's en adresbereiken van Office 365 ](https://docs.microsoft.com/microsoftteams/connectivity-issues) toegankelijk zijn.

- Log in met uw beheerdersaccount en controleer uw [ Servicestatusdashboard ](https://docs.microsoft.com/office365/enterprise/view-service-health) om te controleren of er geen storing of serviceafname is.

 - Als laatste stap kunt u proberen de cache van uw Teams-cliënt te wissen:

    1.  Sluit de Microsoft Teams-desktopclient volledig af. U kunt met de rechtermuisknop op ** Teams ** klikken in het pictogramvak en op ** Afsluiten ** klikken, of Taakbeheer uitvoeren en het proces volledig beëindigen.

    2.  Ga naar Verkenner en typ % appdata% \Microsoft\teams in.

    3.  Eenmaal in de directory ziet u enkele van de volgende mappen:

         - Ga vanuit ** Application Cache ** naar Cache en verwijder alle bestanden op de Cache-locatie: % appdata%\Microsoft\teams\applicationcache\cache.

        - Verwijder vanuit ** Blob_storage ** alle bestanden: % appdata%\Microsoft\teams\blob_storage.

        - Verwijder vanuit ** Cache ** alle bestanden: % appdata%\Microsoft\teams\Cache.

        - Verwijder vanuit ** databases ** alle bestanden: % appdata%\Microsoft\teams\databases.

        - Verwijder vanuit ** GPUCache ** alle bestanden: % appdata%\Microsoft\teams\GPUCache.

        - Verwijder vanuit ** IndexedDB ** alle bestanden: % appdata%\Microsoft\teams\IndexedDB.

        - Verwijder vanuit **Local Storage ** alle bestanden: % appdata%\Microsoft\teams\Local Storage.

        - Verwijder vanuit **tmp ** alle bestanden: %appdata%\Microsoft\teams\tmp.

    4. Start uw Teams-cliënt opnieuw op.
