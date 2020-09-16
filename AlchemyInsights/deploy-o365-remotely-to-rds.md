---
title: Microsoft 365-apps voor Enterprise voor gedeeld gebruik op RDS, Terminal Server of VDI implementeren
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745530"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Microsoft 365-apps voor Enterprise voor gedeeld gebruik op RDS, Terminal Server of VDI implementeren

Microsoft 365-Apps implementeren voor Enterprise met extern bureaublad-services (RDS), eerder met de naam Terminal Services:
- U moet beschikken over een Microsoft 365 voor bedrijven-abonnement of een Office 365-abonnement dat Microsoft 365-apps voor Enterprise bevat, zoals Office 365 Enterprise E3 of Enterprise E5.
   > [!NOTE] 
   > De Microsoft 365-apps voor bedrijven en Microsoft 365 Business Premium Standard-abonnementen zijn niet inbegrepen in Microsoft 365-apps voor Enterprise.
- U dient de [Activering van de gedeelde computer](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)in te schakelen.

> [!NOTE]
> U kunt ook [Microsoft ondersteuning en herstel ondersteuning](https://aka.ms/SaRA_OfficeSCA_M365Portal) voor het installeren van microsoft 365-apps voor Enterprise downloaden en uitvoeren in de modus voor activering van de gedeelde computer.

Zie voor meer informatie over de installatie-instructies en richtlijnen voor aangepaste installaties met behulp van het Office-implementatieprogramma [Microsoft 365-Apps implementeren voor Enterprise met behulp van extern bureaublad services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Fouten oplossen met betrekking tot de activering van gedeelde computers:
- Zie voor meer informatie [over het oplossen van problemen met gedeelde computeractivering voor Microsoft 365-apps voor ondernemingen](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Zie [Activeringsstatus van Microsoft 365-apps voor ondernemingen opnieuw instellen](https://go.microsoft.com/fwlink/?linkid=2109218).

Voer de volgende stappen uit als u Microsoft 365-apps voor Enterprise wilt installeren via het Microsoft 365-Beheercentrum, met de ***Standaardinstellingen voor installeren***:

1.    Controleren welk abonnement u hebt. [Meer informatie](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Overschakelen naar een ander abonnement, indien nodig. [Meer informatie](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Als Office al op de RDS-server is geïnstalleerd met andere Microsoft-abonnementen, moet u deze verwijderen. U kunt bijvoorbeeld **Control Panel**  >  **een programma verwijderen**via het Configuratiescherm. Verwijder met de [Microsoft-ondersteunings-en herstel assistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) als u problemen ondervindt.
4.    Meld u op de RDS-server aan bij het Microsoft 365-Beheercentrum met uw beheerdersaccount en [Installeer Microsoft 365-apps voor Enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5.    Wanneer Office is geïnstalleerd, kunt u geen Office-toepassingen ***openen of u aanmelden*** .
6.    Schakel op de RDS-server het activeren van activerings computers in door het register als volgt te bewerken:
   1. Klik met de rechtermuisknop op de Windows-knop in de linkerbenedenhoek van het scherm en selecteer **uitvoeren**. Typ in het vak Openen de opdracht **regedit**en klik vervolgens op **OK**.
   2. Selecteer **Ja** wanneer u wordt gevraagd of u de Register-editor wilt toestaan om wijzigingen op uw apparaat aan te brengen.
   3. In de Register-editor voegt u een tekenreekswaarde van **SharedComputerLicensing** met de instelling 1 onder HKEY_LOCAL_MACHINE \Software\Microsoft \Office\ClickToRun\Configuration.
   4. Meld u op de RDS-server aan ***als een eindgebruiker*** en [Controleer of de activering voor gedeelde computers is ingeschakeld voor Microsoft 365-apps voor ondernemingen](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

