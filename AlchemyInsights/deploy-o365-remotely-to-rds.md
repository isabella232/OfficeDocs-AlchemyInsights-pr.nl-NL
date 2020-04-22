---
title: Microsoft 365 Apps voor bedrijven implementeren voor gedeeld gebruik op RDS, Terminal Server of VDI
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
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704700"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Microsoft 365 Apps voor bedrijven implementeren voor gedeeld gebruik op RDS, Terminal Server of VDI

Ga als lid van Microsoft 365 Apps for enterprise met Remote Desktop Services (RDS), voorheen Terminal Services:
- U moet een Microsoft 365 For Business-abonnement of een Office 365-abonnement hebben dat Microsoft 365 Apps voor bedrijven bevat, zoals Office 365 Enterprise E3 of Enterprise E5.
   > [!NOTE] 
   > De Microsoft 365 Apps for Business en Microsoft 365 Business Premium Standard-abonnementen bevatten geen Microsoft 365 Apps voor bedrijven.
- U moet [de activering van gedeelde computers](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)inschakelen.

> [!NOTE]
> U de [Microsoft Support- en Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) ook downloaden en uitvoeren om Microsoft 365 Apps voor bedrijven te installeren in de activeringsmodus voor gedeelde computers.

Zie [Microsoft 365 Apps voor bedrijven implementeren met Remote Desktop Services voor](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)meer informatie over vereisten, installatie-instructies en richtlijnen voor aangepaste installaties met behulp van het Office Deployment Tool.

Ga als het gaat om fouten in verband met de activering van gedeelde computers op te lossen:
- Zie [Problemen met de activering van gedeelde computers oplossen voor Microsoft 365 Apps voor bedrijven](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Zie [Activeringsstatus van Microsoft 365-apps voor ondernemingen opnieuw instellen](https://go.microsoft.com/fwlink/?linkid=2109218).

Als u Microsoft 365 Apps voor bedrijven op RDS wilt installeren vanuit het Microsoft 365-beheercentrum, ***dat standaardinstallatie-instellingen gebruikt,*** gebruikt u de volgende stappen:

1.    Controleer welk abonnement je hebt. [Meer informatie](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Schakel indien nodig over naar een ander abonnement. [Meer informatie](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Als Office al is geïnstalleerd op de RDS-server met andere Microsoft-abonnementen, verwijdert u deze. Bijvoorbeeld door naar **Configuratiescherm** > te gaan**Een programma verwijderen.** Verwijder met [Microsoft Support en Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) als u problemen ondervindt.
4.    Meld u op de RDS-server aan bij het Microsoft 365-beheercentrum met uw beheerdersaccount en [installeer Microsoft 365 Apps voor bedrijven.](https://portal.office.com/OLS/MySoftware.aspx)
5.    Nadat Office is geïnstalleerd, ***opent of meldt u zich niet*** aan bij Office-toepassingen.
6.    Schakel op de RDS-server de activering van gedeelde computers in door het register te bewerken door de volgende stappen te volgen:
   1. Klik met de rechtermuisknop op de Windows-knop in de linkerbenedenhoek van het scherm en selecteer **Uitvoeren**. Typ **regedit**in het vak Openen en selecteer **OK**.
   2. Selecteer **Ja** wanneer u wordt gevraagd om de registereditor toe te staan wijzigingen aan te brengen in uw apparaat.
   3. Voeg in de registereditor een tekenreekswaarde van **SharedComputerLicensing** toe met een instelling van 1 onder HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Meld u op de ***RDS-server aan als eindgebruiker*** en [controleer of de activering van gedeelde computers is ingeschakeld voor Microsoft 365 Apps for Enterprise.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)

