---
title: Implementatie van Microsoft 365-apps voor ondernemingen voor gedeeld gebruik op RDS, Terminal Server of VDI
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
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/01/2021
ms.locfileid: "60041001"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementatie van Microsoft 365-apps voor ondernemingen voor gedeeld gebruik op RDS, Terminal Server of VDI

Als u Microsoft 365-apps Extern bureaublad Services (RDS), voorheen Terminal Services, wilt implementeren, moet u het volgende doen:

- Gebruik de eenvoudige oplossing om TLS 1.2 standaard in te stellen als u een oudere versie van Windows gebruikt (bijvoorbeeld Windows 7 SP1, Windows Server 2008 R2). Zie Bijwerken om [TLS 1.1 en TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)in te stellen als standaardveilige protocollen in WinHTTP in Windows. 
- Hebt u een abonnement met Microsoft 365-apps voor ondernemingen (voorheen Office 365 Plus). Bijvoorbeeld Office 365 E3 of Microsoft 365 E5 of een abonnement met de bureaubladversie van Project of Visio, zoals Project Abonnement 3 of Visio Abonnement 2, of het Microsoft 365 Business Premium-abonnement, dat ook Microsoft 365-apps voor bedrijven.
- Activering van gedeelde computer inschakelen. Zie Overzicht van gedeelde [computeractivering](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)voor Microsoft 365-apps.

**Opmerking:** Als u Microsoft 365-apps in de activeringsmodus voor gedeelde computer wilt installeren, downloadt en gebruikt u de [Microsoft-Ondersteunings- en herstelassistent.](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds) Zie Implementatieprogramma's implementeren Microsoft 365-apps extern bureaublad voor meer informatie over vereisten, installatie-instructies en richtlijnen voor het aanpassen van installaties met behulp van het Office [Implementatieprogramma.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

Zie het volgende als u fouten met betrekking tot de activering van gedeelde computer wilt oplossen:

- [Problemen met de activering van gedeelde computer oplossen voor Microsoft 365-apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Activeringsstatus van Microsoft 365-apps voor bedrijven opnieuw instellen](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Als u een Microsoft 365-apps op RDS wilt installeren vanaf de Microsoft 365-beheercentrum, waarbij standaardinstellingen voor installatie worden gebruikt, volgt u de volgende stappen:

1. Controleer welk Microsoft 365 hebt. Zie Welk abonnement heb ik? voor [meer informatie.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

1. Schakel indien nodig over naar een ander Microsoft 365 plan. Zie Upgraden naar [een ander abonnement voor meer informatie.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Als Microsoft 365-apps al is geïnstalleerd op de RDS-server met andere niet-compatibele abonnementen, verwijdert u deze door naar configuratiescherm Een programma   >  **te verwijderen.** Als er problemen zijn, verwijdert [](https://aka.ms/SARA-OfficeUninstall-Alchemy)u de installatie door Microsoft-Ondersteunings- en herstelassistent.

1. Meld u op de RDS-server aan bij de Microsoft 365-beheercentrum met uw beheerdersaccount en [installeer Office.](https://portal.office.com/OLS/MySoftware.aspx)

   Nadat Office is geïnstalleerd, hoeft u zich niet te openen of aan te melden bij Office toepassingen.

1. Schakel op de RDS-server gedeelde computeractivering in door het register te bewerken:

   1. Klik met de rechtermuisknop op Windows knop in de linkerbenedenhoek van het scherm en selecteer **Uitvoeren.** Typ in het vak Openen **regedit** en klik vervolgens op **OK**.

   1. Wanneer u wordt gevraagd om registereditor toe te staan wijzigingen aan te brengen op uw apparaat, selecteert u **Ja.**

   1. Voeg in de registereditor onder HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration een tekenreekswaarde van **SharedComputerLicensing** toe met een instelling **van 1** .

1. Meld u op de RDS-server aan als eindgebruiker en controleer of gedeelde computeractivering is ingeschakeld voor Microsoft 365-apps. 

   Zie Controleren [of activering van gedeelde computer is ingeschakeld](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)voor Microsoft 365-apps.