---
title: Microsoft 365-apps voor bedrijven implementeren voor gedeeld gebruik op RDS, Terminal Server of VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507581"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Microsoft 365-apps voor bedrijven implementeren voor gedeeld gebruik op RDS, Terminal Server of VDI

Microsoft 365-apps voor bedrijven implementeren met Behulp van Extern bureaublad-services (RDS), voorheen Terminal Services:
- U moet beschikken over een Microsoft 365 Voor Bedrijven-abonnement of een Office 365-abonnement dat Microsoft 365-apps voor bedrijven bevat, zoals Office 365 Enterprise E3 of Enterprise E5.
   > [!NOTE] 
   > De Microsoft 365 Apps for Business en Microsoft 365 Business Premium Standard-abonnementen bevatten geen Microsoft 365-apps voor bedrijven.
- U moet [gedeelde computeractivering](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)inschakelen.

> [!NOTE]
> U ook de Microsoft Support and [Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) downloaden en uitvoeren om Microsoft 365 Apps for enterprise te installeren in de activeringsmodus van gedeelde computer.

Zie [Microsoft 365-apps voor bedrijven implementeren met Behulp van Extern bureaublad-services voor](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)meer informatie over vereisten, installatieinstructies en richtlijnen voor aangepaste installaties.

Fouten in verband met activering van gedeelde computer oplossen:
- Zie [Problemen oplossen met gedeelde computeractivering voor Microsoft 365 Apps voor bedrijven](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Zie [Activeringsstatus van Microsoft 365-apps voor ondernemingen opnieuw instellen](https://go.microsoft.com/fwlink/?linkid=2109218).

Als u Microsoft 365 Apps voor bedrijven op RDS wilt installeren vanuit het Microsoft 365-beheercentrum, ***dat standaardinstallatie-instellingen gebruikt,*** voert u de volgende stappen uit:

1.    Controleer welk abonnement je hebt. [Meer informatie](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Schakel indien nodig over naar een ander abonnement. [Meer informatie](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Als Office al op de RDS-server is geïnstalleerd met andere Microsoft-abonnementen, verwijdert u deze. Bijvoorbeeld door naar **het Configuratiescherm**te gaan  >  **Een programma verwijderen.** Verwijder het verwijderen met [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) als u problemen ondervindt.
4.    Meld u op de RDS-server aan bij het Microsoft 365-beheercentrum met uw beheerdersaccount en [installeer Microsoft 365 Apps voor bedrijven.](https://portal.office.com/OLS/MySoftware.aspx)
5.    Nadat Office is geïnstalleerd, ***opent u office-toepassingen niet of meldt u zich niet aan.***
6.    Schakel op de RDS-server gedeelde computeractivering in door het register te bewerken door de volgende stappen te volgen:
   1. Klik met de rechtermuisknop op de Windows-knop linksonder in het scherm en selecteer **Uitvoeren**. Typ **regedit in**het vak Openen en selecteer **vervolgens OK**.
   2. Selecteer **Ja** wanneer u wordt gevraagd om registereditor toe te staan wijzigingen aan te brengen in uw apparaat.
   3. Voeg in de registereditor een tekenreekswaarde van **SharedComputerLicensing** toe met een instelling van 1 onder HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Meld u op de RDS-server ***aan als eindgebruiker*** en controleer of [gedeelde computeractivering is ingeschakeld voor Microsoft 365 Apps voor bedrijven](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

