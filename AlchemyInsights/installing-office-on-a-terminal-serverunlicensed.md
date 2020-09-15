---
title: Office installeren op een Terminal Server-zonder licentie
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
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663112"
---
# <a name="installing-office-on-a-terminal-server"></a>Office installeren op een Terminal Server

Voor het implementeren van Microsoft 365-apps voor Enterprise op een Windows Server met extern bureaublad-services (RDS), eerder met de naam Terminal Services:
  
- U moet een Microsoft 365-abonnement hebben dat Microsoft 365-apps voor Enterprise bevat, zoals Office 365 Enterprise E3 of Enterprise E5. De Microsoft 365 apps for Business and Microsoft 365 apps for Business Premium-abonnementen bevatten geen Microsoft 365-apps voor Enterprise.

- U dient de activering van de [gedeelde computer](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)in te schakelen.

Voer de volgende stappen uit als u Microsoft 365-apps voor Enterprise op RDS wilt installeren via het Microsoft 365-Beheercentrum, met de ***Standaardinstellingen voor installeren***.

> [!TIP]
> U kunt ook [Microsoft ondersteuning en herstel ondersteuning](https://aka.ms/SaRA_OfficeSCA_M365Portal) voor het installeren van microsoft 365-apps voor Enterprise downloaden en uitvoeren in de modus voor activering van de gedeelde computer.
  
1. Controleer wat Microsoft 365-abonnement u hebt. [Meer informatie](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Overschakelen naar een ander abonnement van Microsoft 365, indien nodig. [Meer informatie](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Als Office al op de RDS-server is geïnstalleerd met andere Microsoft 365-abonnementen, verwijdert u de app. U kunt bijvoorbeeld een programma verwijderen via het Configuratiescherm \> . Verwijder met de [Microsoft-ondersteunings-en herstel assistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) als u problemen ondervindt.

4. Meld u op de RDS-server aan bij het Microsoft 365-Beheercentrum met uw beheerdersaccount en [Installeer Microsoft 365-apps voor Enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Wanneer Office is geïnstalleerd, kunt u geen Office-toepassingen ***openen of u aanmelden*** .

6. Schakel op de RDS-server het activeren van activerings computers in door het register als volgt te bewerken:

1. Klik met de rechtermuisknop op de Windows-knop in de linkerbenedenhoek van het scherm en selecteer uitvoeren. Typ in het vak Openen de opdracht **regedit**en klik vervolgens op OK.

2. Selecteer Ja wanneer u wordt gevraagd of u de Register-editor wilt toestaan om wijzigingen op uw apparaat aan te brengen.

3. In de Register-editor voegt u een tekenreekswaarde van **SharedComputerLicensing** met de instelling 1 onder HKEY_LOCAL_MACHINE \Software\Microsoft \Office\ClickToRun\Configuration.

7. Meld u op de RDS-server aan ***als een eindgebruiker*** en [Controleer of de activering voor gedeelde computers is ingeschakeld voor Microsoft 365-apps voor ondernemingen](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Zie voor meer informatie over de installatie-instructies en richtlijnen voor aangepaste installaties met behulp van het Office-implementatieprogramma [Microsoft 365-Apps implementeren voor Enterprise met behulp van extern bureaublad services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Zie problemen met de activering van een [gedeelde computer voor Microsoft 365-apps voor bedrijven oplossen](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)voor meer informatie over het oplossen van problemen met de activering van een gedeelde computer.
  