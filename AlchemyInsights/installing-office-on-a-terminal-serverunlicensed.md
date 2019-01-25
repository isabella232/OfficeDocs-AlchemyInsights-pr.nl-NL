---
title: Office installeren op een Terminal Server - licentie
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29465369"
---
# <a name="installing-office-on-a-terminal-server"></a>Office installeren op een Terminal-Server

Voorheen Terminal Services voor het implementeren van Office 365 ProPlus op een Windows-Server met behulp van extern bureaublad-Services (RDS):
  
- U hebt een plan Office 365 met Office 365 ProPlus, zoals Office 365 Enterprise E3 of Enterprise E5. De Office 365 Business en Office 365 Business Premium plannen bevatten geen Office 365 ProPlus.
    
- U moet [gedeelde computer activeren](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)inschakelen.
    
Als u wilt dat Office 365 ProPlus installeren op RDS vanuit de Office 365 portal ** *die gebruikmaakt van standaard installatie-instellingen* **, als volgt te werk: 
  
1. Controleer wat u hebt Office 365-plan. [Informatie over hoe](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Indien nodig, overschakelen naar een ander Office 365 plan. [Informatie over hoe](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Als Office al is geïnstalleerd op de RDS-server met behulp van Office 365 plannen, verwijderen. Bijvoorbeeld door te gaan naar het Configuratiescherm \> een programma verwijderen. Verwijderen met behulp van [Microsoft-ondersteuning en herstel-assistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) als u in de problemen. 
    
4. Log in op de RDS-server aan met uw administrator-account en het [installeren van Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)Office 365 portal.
    
5. Nadat Office is geïnstalleerd, ** *niet openen of inloggen* ** aan alle Office-toepassingen. 
    
6. Inschakelen op de server met RDS gedeelde computer activeren door het bewerken van het register door de volgende stappen:
    
1. Klik met de rechtermuisknop op de Windows-knop in de linkerbenedenhoek van het scherm en selecteer uitvoeren. Typ **regedit**in het vak openen en klik vervolgens op OK. 
    
2. Selecteer Ja wanneer u wordt gevraagd om de Register-Editor om uw apparaat te wijzigen.
    
3. Een string-waarde van **SharedComputerLicensing** in de Register-Editor toevoegen met de waarde 1 onder HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. Op de server met RDS ** *Aanmelden als een eindgebruiker* ** en [Controleer of gedeelde computer activeren voor Office 365 ProPlus is ingeschakeld](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Zie [Implementatie van Office 365 ProPlus met behulp van extern bureaublad-Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)voor meer informatie over vereisten, installatie-instructies en richtlijnen voor aangepaste installaties met behulp van de Office Deployment Tool.
  
Voor het oplossen van fouten met betrekking tot de gedeelde computer activeren, Zie [problemen oplossen met het activeren van Office 365 ProPlus gedeelde computer](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

