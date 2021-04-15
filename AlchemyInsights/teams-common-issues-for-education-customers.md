---
title: Veelvoorkomende problemen van Teams voor Education-klanten
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
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 893c8cacaf089932014ba7a3ea6122d17da38cdd
ms.sourcegitcommit: ef7ec42aba3c06aa8966dfac71cec18c08e7acf8
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/13/2021
ms.locfileid: "51692389"
---
# <a name="teams-common-issues-for-education-customers"></a>Veelvoorkomende problemen van Teams voor Education-klanten

**Voor Education-klanten:**

Als u hulp nodig hebt bij de implementatie van Teams om extern leren te ondersteunen, gaat u naar het [FastTrack Center](https://www.microsoft.com/fasttrack) om een aanvraag te verzenden. Zie de volgende veelvoorkomende problemen voor Education-klanten van Teams:

- Als u de melding '**U mist veel**' ziet bekijk dan [Microsoft Teams inschakelen voor uw school](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). In EDU-tenants is Microsoft Teams niet standaard ingeschakeld, u zult deze eerst in moeten schakelen.

- **Nog niet bekend met Teams?** Bekijk [Op afstand onderwijzen en leren in Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) voor de meest recente richtlijnen voor het instellen van uw school, lesplannen, virtuele vergaderingen en het delen van inhoud met leerlingen/studenten.

- Wanneer deze optie is ingeschakeld, kunnen uw gebruikers Teams uitvoeren door [desktop](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client)- en [mobiele clients](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients) te installeren of via de browser op https://teams.microsoft.com.

- **Toegang voor gasten in Teams inschakelen:** bekijk de [Controlelijst voor gasttoegang in Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist) en zorg ervoor dat alle stappen zijn voltooid.
    - [Meer informatie over Toegang voor gasten in Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Configuratie: controlelijst voor toegang voor gasten voor Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Hoe een gast lid wordt van een team](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams-vergaderingen en inbellen**: hulp nodig bij het inschakelen of het instellen van audiovergaderingen in Microsoft Teams?? Is deze gebruiker onlangs gemaakt? Als dat het geval is, moet u 2 tot 24 uur wachten voordat de instellingen van kracht worden. U kunt als volgt controleren of de gebruiker een licentie heeft voor audiovergaderingen en een standaard betaald nummer:
    1. Ga naar Actieve gebruikers en selecteer de betreffende gebruiker.
    2. Afhankelijk van de versie van het beheercentrum kiest u **Licenties en apps** of klikt u op **Bewerken** bij **Productlicenties**.
    3. Controleer of de gebruiker licenties heeft geselecteerd voor Audiovergaderingen, Microsoft Teams en Skype voor Bedrijven Online (abonnement 2).
    4. Gebruikers-beheercentra klik op **Alles weergeven** en vervolgens op **Teams**.
    5. Klik op **Legacy-portaal** in het Microsoft Teams-beheercentrum.
    6. Klik in het Skype voor Bedrijven-beheercentrum op **Audiovergaderingen** en vervolgens op **Gebruikers**.
    7. Selecteer de gewenste gebruiker en controleer of de gebruiker een standaard betaald nummer heeft.

    Zie [Microsoft Teams Calling Plans](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) (Belabonnementen voor Microsoft Teams) of bel het Microsoft Commerce-factureringsteam voor hulp bij vragen over licenties voor meer informatie.

    Aanvullende resources

    - [Vergaderingen en conferenties in Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Audio Conferencing](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365) (Audiovergaderingen)

- **Beleidsregels voor vergaderingen**: u gebruikt beleidsregels voor vergaderingen om te bepalen welke functies beschikbaar zijn voor deelnemers aan vergaderingen die zijn gepland door gebruikers in uw organisatie. Wanneer u een beleid hebt gemaakt en u uw wijzigingen hebt aangebracht, kunt u gebruikers toewijzen aan het beleid.

    - **Beleidsregels voor vergaderingen wijzigen of maken**: als u beleidsregels voor vergaderingen wilt wijzigen of maken, gaat u naar het **Microsoft Teams-beheercentrum > Vergaderingen > Beleidsregels voor vergaderingen**. Selecteer een beleid in de lijst of klik op **Toevoegen**. Als u een nieuw beleid wilt maken, voegt u een naam en beschrijving toe. De naam mag geen speciale tekens bevatten en mag niet langer zijn dan 64 tekens. Kies de gewenste instellingen en klik op **Opslaan**. 
    
        Stel dat u een groot aantal gebruikers hebt en u wilt de hoeveelheid bandbreedte beperken die nodig is voor de vergadering. U maakt dan een nieuw aangepast beleid met bijvoorbeeld de naam 'Beperkte bandbreedte' en schakelt de volgende instellingen uit:

        Onder **Audio en video**:
        - Schakel de optie **Cloudopnamen toestaan** uit.
        - Schakel **IP-video toestaan** uit.

        Onder **Inhoud delen**:

        - Schakel de modus Scherm delen uit.
        - Schakel **Whiteboard toestaan** uit.
        - Schakel **Gedeelde notities toestaan** uit.

        Vervolgens kunt u **beleid toewijzen aan de gebruikers**:

    1. Ga in het linkernavigatiegedeelte van het Microsoft Teams-beheercentrum naar **Gebruikers** en klik vervolgens op de gebruiker.
    2. Selecteer de gebruiker door links van de gebruikersnaam te klikken en klik vervolgens op **Instellingen bewerken**.
    3. Selecteer onder **Beleidsregels voor vergaderingen** het beleid dat u wilt toewijzen en klik vervolgens op **Toepassen**.

    Zie [Gebruikersinstellingen in Teams bulksgewijs bewerken](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk) als u beleidsregels wilt toewijzen aan meerdere gebruikers tegelijk.

    Of u doet het volgende:
    1. Ga in de linkernavigatiebalk van het Microsoft Teams-beheercentrum naar **Vergaderingen > Beleidsregels voor vergaderingen**.
    2. Selecteer het beleid door links van de beleidsnaam te klikken.
    3. Klik op **Gebruikers beheren**.
    4. Zoek in het deelvenster **Gebruikers beheren** op weergavenaam of op gebruikersnaam naar de gebruiker, selecteer de naam en selecteer vervolgens **Toevoegen**. Herhaal deze stap voor elke gebruiker die u wilt toevoegen.
    5. Als u klaar bent met het toevoegen van gebruikers, klikt u op **Opslaan**.

- **Problemen met een ontbrekend toetsenblok oplossen**:
    - Zorg ervoor dat de gebruiker een [Teams-licentie](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses) is toegewezen.
    - Zorg ervoor dat de gebruiker een [belabonnement](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page) is toegewezen.
    - Schakel de gebruikers in voor [Enterprise Voice](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Aanmeldingsproblemen in Teams oplossen**: controleer eerst of de [Microsoft Teams-service in orde is](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Controleer vervolgens op veelvoorkomende foutcodes en bekijk [Waarom kan ik me niet aanmelden bij Microsoft Teams?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f) Mogelijk moet u ook [Identiteitsmodellen en verificatie in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication) bekijken.
