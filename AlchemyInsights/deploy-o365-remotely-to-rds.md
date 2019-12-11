---
title: Office 365 ProPlus implementeren voor gedeeld gebruik op RDS, Terminal Server of VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959455"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Office 365 ProPlus implementeren voor gedeeld gebruik op RDS, Terminal Server of VDI

Office 365 ProPlus implementeren met extern bureaublad-services (RDS), voorheen Terminal Services genoemd:
- U moet beschikken over een Microsoft 365 voor Business-abonnement of een Office 365-abonnement met Office 365 ProPlus, zoals Office 365 Enterprise E3 of Enterprise E5.
   > [!NOTE] 
   > De Office 365 Business en Office 365 Business Premium-abonnementen bevatten geen Office 365 ProPlus.
- U moet de [Activering van gedeelde computers](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)inschakelen.

> [!NOTE]
> U ook de [Microsoft-ondersteunings-en Herstelassistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) downloaden en uitvoeren om Office 365 ProPlus te installeren in de activerings modus voor gedeelde computers.

Zie voor meer informatie over vereisten, installatie-instructies en richtlijnen voor aangepaste installaties met behulp van de Office Deployment Tool [office 365 ProPlus implementeren met behulp van extern bureaublad-services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Fouten met betrekking tot de activering van gedeelde computers oplossen:
- Zie problemen [met gedeelde computer activering voor Office 365 ProPlus oplossen](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Zie de [activeringsstatus van Office 365 ProPlus opnieuw instellen](https://go.microsoft.com/fwlink/?linkid=2109218).

Als u wilt installeren van Office 365 ProPlus op RDS van de Microsoft 365 Admin Center, ***die gebruikmaakt van standaardinstallatie-instellingen***, gebruikt u de volgende stappen uit:

1.  Controleer welk Office 365-abonnement u hebt. [Meer informatie](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Schakel indien nodig naar een ander Office 365-abonnement. [Meer informatie](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Als Office al is geïnstalleerd op de RDS-server met behulp van een andere Office 365-abonnementen, verwijdert u deze. Bijvoorbeeld, door te gaan naar het **Configuratiescherm** > **een programma verwijderen**. Verwijder met [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) als u problemen ondervindt.
4.  Meld u op de RDS-server aan bij het Microsoft 365 Admin Center met uw beheerdersaccount en [Installeer Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Nadat Office is geïnstalleerd, ***niet openen of aanmelden*** bij een Office-toepassingen.
6.  Schakel op de RDS-server de activering van gedeelde computers in door het register te bewerken door de volgende stappen uit te voeren:
   1. Klik met de rechtermuisknop op de knop Windows linksonder in het scherm en selecteer **uitvoeren**. Typ **regedit**in het vak openen en selecteer vervolgens **OK**.
   2. Selecteer **Ja** wanneer u wordt gevraagd de Register-editor toe te staan wijzigingen aan te brengen in uw apparaat.
   3. In de Register-editor, voeg een tekenreekswaarde van **Sharedcomputerlicensing** met een instelling van 1 onder HKEY_LOCAL_MACHINE \Software\microsoft \Office\ClickToRun\Configuration.
   4. Meld u op de RDS-server aan ***als eindgebruiker*** en [Controleer of de activering van gedeelde computers is ingeschakeld voor Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

