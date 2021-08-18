---
title: Office installeren op een Terminal Server - Zonder licentie
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321994"
---
# <a name="installing-office-on-a-terminal-server"></a>Installatie van Office op een terminalserver

Voor het implementeren van Microsoft 365-apps voor ondernemingen op een Windows Server met RDS (Remote Desktop Services), voorheen Terminal Services genoemd:
  
- U moet een abonnement Microsoft 365 met Microsoft 365-apps voor ondernemingen, zoals Office 365 Enterprise E3 of Enterprise E5. De Microsoft 365-apps voor bedrijven en Microsoft 365-apps voor bedrijven Premium bevatten geen Microsoft 365-apps voor ondernemingen.

- U moet activering van gedeelde [computer inschakelen.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Als u een Microsoft 365-apps voor ondernemingen op RDS wilt installeren vanaf de ***Microsoft 365-beheercentrum,*** waarbij standaardinstellingen voor installatie worden gebruikt, gebruikt u de volgende stappen.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Controleer welk Microsoft 365 hebt. [Meer informatie over hoe](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Schakel indien nodig over naar een ander Microsoft 365 abonnement. [Meer informatie over hoe](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Als Office al is geïnstalleerd op de RDS-server met andere Microsoft 365, verwijdert u deze. Ga bijvoorbeeld naar Configuratiescherm \> Een programma verwijderen. Verwijder het gebruik [van Microsoft Ondersteunings- en herstelassistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) als er problemen zijn.

4. Meld u op de RDS-server aan bij de Microsoft 365-beheercentrum met uw beheerdersaccount en [installeer Microsoft 365-apps voor ondernemingen.](https://portal.office.com/OLS/MySoftware.aspx)

5. Nadat Office is geïnstalleerd, hoeft u zich niet ***te openen*** of aan te melden bij Office toepassingen.

6. Schakel op de RDS-server gedeelde computeractivering in door het register te bewerken door de volgende stappen uit te voeren:

1. Klik met de rechtermuisknop Windows in de linkerbenedenhoek van het scherm en selecteer Uitvoeren. Typ **regedit** in het vak Openen en selecteer OK.

2. Selecteer Ja wanneer u wordt gevraagd om registereditor toe te staan wijzigingen aan te brengen op uw apparaat.

3. Voeg in de registereditor een tekenreekswaarde van **SharedComputerLicensing** toe met een instelling van 1 onder HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Meld u op de  RDS-server aan als eindgebruiker en controleer of gedeelde computeractivering is ingeschakeld voor [Microsoft 365-apps voor ondernemingen.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Zie Implementeer Microsoft 365-apps voor ondernemingen met behulp van Remote Desktop Services voor meer informatie over vereisten, installatie-instructies en richtlijnen voor aangepaste installaties met behulp van het Office Deployment [Tool.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Zie Problemen oplossen met gedeelde [computeractivering](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)voor Microsoft 365-apps voor ondernemingen.
  