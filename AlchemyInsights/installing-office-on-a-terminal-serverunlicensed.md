---
title: Office installeren op een terminalserver - Zonder licentie
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508623"
---
# <a name="installing-office-on-a-terminal-server"></a>Office installeren op een terminalserver

Voor het implementeren van Microsoft 365-apps voor bedrijven op een Windows Server met Extern bureaublad-services (RDS), voorheen Terminal Services:
  
- U moet een Microsoft 365-abonnement hebben dat Microsoft 365 Apps voor bedrijven bevat, zoals Office 365 Enterprise E3 of Enterprise E5. De Microsoft 365 Apps for Business en Microsoft 365 Apps for business Premium-abonnementen bevatten geen Microsoft 365 Apps voor bedrijven.

- U moet [gedeelde computeractivering](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)inschakelen.

Als u Microsoft 365 Apps voor bedrijven op RDS wilt installeren vanuit het Microsoft 365-beheercentrum, ***dat standaardinstallatie-instellingen gebruikt,*** voert u de volgende stappen uit.

> [!TIP]
> U ook de Microsoft Support and [Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) downloaden en uitvoeren om Microsoft 365 Apps for enterprise te installeren in de activeringsmodus van gedeelde computer.
  
1. Controleer welk Microsoft 365-abonnement u hebt. [Meer informatie over hoe](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Schakel indien nodig over naar een ander Microsoft 365-abonnement. [Meer informatie over hoe](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Als Office al op de RDS-server is geïnstalleerd met andere Microsoft 365-abonnementen, verwijdert u deze. Bijvoorbeeld door naar het Configuratiescherm te gaan \> Een programma verwijderen. Verwijder het verwijderen met [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) als u problemen ondervindt.

4. Meld u op de RDS-server aan bij het Microsoft 365-beheercentrum met uw beheerdersaccount en [installeer Microsoft 365 Apps voor bedrijven.](https://portal.office.com/OLS/MySoftware.aspx)

5. Nadat Office is geïnstalleerd, ***opent u office-toepassingen niet of meldt u zich niet aan.***

6. Schakel op de RDS-server gedeelde computeractivering in door het register te bewerken door de volgende stappen te volgen:

1. Klik met de rechtermuisknop op de Windows-knop in de linkerbenedenhoek van het scherm en selecteer Uitvoeren. Typ **regedit in**het vak Openen en selecteer OK.

2. Selecteer Ja wanneer u wordt gevraagd om registereditor toe te staan wijzigingen aan te brengen in uw apparaat.

3. Voeg in de registereditor een tekenreekswaarde van **SharedComputerLicensing** toe met een instelling van 1 onder HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Meld u op de RDS-server ***aan als eindgebruiker*** en controleer of [gedeelde computeractivering is ingeschakeld voor Microsoft 365 Apps voor bedrijven](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Zie [Microsoft 365-apps implementeren voor bedrijven implementeren met Behulp van Extern bureaublad-services voor](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)meer informatie over vereisten, installatieinstructies en richtlijnen voor aangepaste installaties met behulp van het Office Deployment Tool.
  
Zie Problemen [oplossen met gedeelde computeractivering voor Microsoft 365 Apps voor bedrijven](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)om fouten met betrekking tot de activering van gedeelde computer op te lossen.
  