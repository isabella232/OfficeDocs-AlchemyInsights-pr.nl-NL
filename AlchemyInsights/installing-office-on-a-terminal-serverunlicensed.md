---
title: Office installeren op een Terminal Server-zonder licentie
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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/25/2019
ms.locfileid: "37205404"
---
# <a name="installing-office-on-a-terminal-server"></a>Office installeren op een Terminal Server

Voor het implementeren van Office 365 ProPlus op een Windows-Server met behulp van extern bureaublad-services (RDS), voorheen genaamd Terminal Services:
  
- U moet beschikken over een Office 365-abonnement met Office 365 ProPlus, zoals Office 365 Enterprise E3 of Enterprise E5. De Office 365 Business en Office 365 Business Premium-abonnementen bevatten geen Office 365 ProPlus.

- U moet de [Activering van gedeelde computers](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)inschakelen.

Als u wilt installeren van Office 365 ProPlus op RDS van de Microsoft 365 Admin Center, ***die gebruikmaakt van standaardinstallatie-instellingen***, gebruikt u de volgende stappen uit.

> [!TIP]
> U ook de [Microsoft-ondersteunings-en Herstelassistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) downloaden en uitvoeren om Office 365 ProPlus te installeren in de activerings modus voor gedeelde computers.
  
1. Controleer welk Office 365-abonnement u hebt. [Leer hoe](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Schakel indien nodig naar een ander Office 365-abonnement. [Leer hoe](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Als Office al is geïnstalleerd op de RDS-server met behulp van een andere Office 365-abonnementen, verwijdert u deze. Bijvoorbeeld, door te gaan naar het configuratie \> scherm een programma verwijderen. Verwijder met [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) als u problemen ondervindt.

4. Meld u op de RDS-server aan bij het Microsoft 365 Admin Center met uw beheerdersaccount en [Installeer Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Nadat Office is geïnstalleerd, ***niet openen of aanmelden*** bij een Office-toepassingen.

6. Schakel op de RDS-server de activering van gedeelde computers in door het register te bewerken door de volgende stappen uit te voeren:

1. Klik met de rechtermuisknop op de Windows-knop in de linkerbenedenhoek van uw scherm en selecteer uitvoeren. Typ **regedit**in het vak openen en selecteer vervolgens OK.

2. Selecteer Ja wanneer u wordt gevraagd de Register-editor toe te staan wijzigingen aan te brengen in uw apparaat.

3. In de Register-editor, voeg een tekenreekswaarde van **Sharedcomputerlicensing** met een instelling van 1 onder HKEY_LOCAL_MACHINE\Software\Microsoft \Office\ClickToRun\Configuration.

7. Meld u op de RDS-server aan ***als eindgebruiker*** en [Controleer of de activering van gedeelde computers is ingeschakeld voor Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Zie voor meer informatie over vereisten, installatie-instructies en richtlijnen voor aangepaste installaties met behulp van de Office Deployment Tool, [office 365 ProPlus implementeren met behulp van extern bureaublad-services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Als u fouten met betrekking tot de activering van gedeelde computers wilt oplossen, raadpleegt u [problemen met gedeelde computer activering voor Office 365 ProPlus oplossen](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  