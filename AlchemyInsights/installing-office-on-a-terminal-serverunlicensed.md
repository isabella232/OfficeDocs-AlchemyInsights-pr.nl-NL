---
title: Kantoor installeren op een terminalserver - zonder licentie
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
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763212"
---
# <a name="installing-office-on-a-terminal-server"></a>Office installeren op een terminalserver

Voor het implementeren van Microsoft 365 Apps for enterprise op een Windows Server met Remote Desktop Services (RDS), voorheen Terminal Services:
  
- U moet een Microsoft 365-abonnement hebben dat Microsoft 365 Apps voor bedrijven bevat, zoals Office 365 Enterprise E3 of Enterprise E5. De Microsoft 365 Apps for Business en Microsoft 365 Apps for business Premium-abonnementen bevatten geen Microsoft 365 Apps voor bedrijven.

- U moet [de activering van gedeelde computers](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)inschakelen.

Als u Microsoft 365 Apps voor bedrijven op RDS wilt installeren vanuit het Microsoft 365-beheercentrum, ***dat standaardinstallatie-instellingen gebruikt,*** gebruikt u de volgende stappen.

> [!TIP]
> U de [Microsoft Support- en Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) ook downloaden en uitvoeren om Microsoft 365 Apps voor bedrijven te installeren in de activeringsmodus voor gedeelde computers.
  
1. Controleer welk Microsoft 365-abonnement u hebt. [Meer informatie over hoe](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Schakel indien nodig over naar een ander Microsoft 365-abonnement. [Meer informatie over hoe](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Als Office al is geïnstalleerd op de RDS-server met andere Microsoft 365-abonnementen, verwijdert u deze. Bijvoorbeeld door naar Configuratiescherm \> te gaan Een programma verwijderen. Verwijder met [Microsoft Support en Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) als u problemen ondervindt.

4. Meld u op de RDS-server aan bij het Microsoft 365-beheercentrum met uw beheerdersaccount en [installeer Microsoft 365 Apps voor bedrijven.](https://portal.office.com/OLS/MySoftware.aspx)

5. Nadat Office is geïnstalleerd, ***opent of meldt u zich niet*** aan bij Office-toepassingen.

6. Schakel op de RDS-server de activering van gedeelde computers in door het register te bewerken door de volgende stappen te volgen:

1. Klik met de rechtermuisknop op de Windows-knop in de linkerbenedenhoek van het scherm en selecteer Uitvoeren. Typ **regedit**in het vak Openen en selecteer OK.

2. Selecteer Ja wanneer u wordt gevraagd om de registereditor toe te staan wijzigingen aan te brengen in uw apparaat.

3. Voeg in de registereditor een tekenreekswaarde van **SharedComputerLicensing** toe met een instelling van 1 onder HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Meld u op de ***RDS-server aan als eindgebruiker*** en [controleer of de activering van gedeelde computers is ingeschakeld voor Microsoft 365 Apps for Enterprise.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)

Zie [Microsoft 365 Apps voor bedrijven implementeren met Remote Desktop Services voor](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)meer informatie over vereisten, installatie-instructies en richtlijnen voor aangepaste installaties met behulp van het Office Deployment Tool.
  
Zie [Problemen met de activering van gedeelde computers oplossen voor microsoft 365 Apps voor bedrijven](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)om fouten in verband met de activering van gedeelde computers op te lossen.
  