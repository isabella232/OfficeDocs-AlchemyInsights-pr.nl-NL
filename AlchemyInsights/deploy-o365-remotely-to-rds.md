---
title: Microsoft 365-apps voor ondernemingen implementeren voor gedeeld gebruik op RDS, Terminal Server of VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200668"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Microsoft 365-apps voor ondernemingen implementeren voor gedeeld gebruik op RDS, Terminal Server of VDI

Microsoft 365-apps voor ondernemingen implementeren met RDS (Remote Desktop Services), voorheen Terminal Services genoemd:

- U moet een Microsoft 365 Voor Bedrijven-abonnement of een Office 365-abonnement hebben met Microsoft 365 Apps voor ondernemingen, zoals Office 365 Enterprise E3 of Enterprise E5.
   > [!NOTE]
   > Microsoft 365 Apps voor Bedrijven en Microsoft 365 Business Standard-abonnementen bevatten geen Microsoft 365-apps voor ondernemingen.
- U moet activering van [gedeelde computer inschakelen.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> U kunt ook de [Microsoft-ondersteunings-](https://aka.ms/SaRA_OfficeSCA_M365Portal) en herstelassistent downloaden en uitvoeren om Microsoft 365 Apps voor ondernemingen te installeren in de activeringsmodus voor gedeelde computer.

Zie [Microsoft 365-apps](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)voor bedrijven implementeren met behulp van Remote Desktop Services voor meer informatie over vereisten, installatie-instructies en richtlijnen voor aangepaste installaties met behulp van het Office-implementatieprogramma.

Fouten met betrekking tot activering van gedeelde computer oplossen:

- Zie [Problemen oplossen met gedeelde computeractivering voor Microsoft 365 Apps voor bedrijven](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Zie [Activeringsstatus van Microsoft 365-apps voor ondernemingen opnieuw instellen](https://go.microsoft.com/fwlink/?linkid=2109218).

Als u Microsoft 365 Apps voor ondernemingen wilt installeren op RDS vanuit het Microsoft 365-beheercentrum, dat standaardinstellingen voor installatie gebruikt, gebruikt u de volgende stappen:

1. Controleer welk abonnement u hebt. [Meer informatie](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Schakel indien nodig over naar een ander abonnement. [Meer informatie](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Als Office al is geïnstalleerd op de RDS-server met andere Microsoft-abonnementen, verwijdert u deze. Ga bijvoorbeeld naar **Configuratiescherm**  >  **Een programma verwijderen.** Verwijder de installatie [met microsoft-ondersteunings- en herstelassistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) als er problemen zijn.
4. Meld u op de RDS-server aan bij het Microsoft 365-beheercentrum met uw beheerdersaccount en [installeer Microsoft 365 Apps voor bedrijven.](https://portal.office.com/OLS/MySoftware.aspx)
5. Nadat Office is geïnstalleerd, ***hoeft u zich niet te openen*** of aan te melden bij Office-toepassingen.
6. Schakel op de RDS-server de activering van gedeelde computer in door het register te bewerken door de volgende stappen uit te voeren:
   1. Klik met de rechtermuisknop op de Windows-knop in de linkerbenedenhoek van het scherm en selecteer **Uitvoeren.** Typ in het vak Openen **regedit** en klik vervolgens op **OK**.
   2. Selecteer **Ja** wanneer u wordt gevraagd om registereditor toe te staan wijzigingen aan te brengen op uw apparaat.
   3. Voeg in de registereditor een tekenreekswaarde van **SharedComputerLicensing** toe met een instelling van 1 onder HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Meld u op de  RDS-server aan als eindgebruiker en controleer of gedeelde computeractivering is ingeschakeld voor [Microsoft 365 Apps voor ondernemingen.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
