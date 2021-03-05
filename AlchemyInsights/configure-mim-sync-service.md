---
title: MIM-synchronisatieservice configureren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481354"
---
# <a name="configure-mim-sync-service"></a>MIM-synchronisatieservice configureren

Microsoft Identity Manager (MIM) Synchronization Service is een onderdeel van MIM. Het is een centrale on-premises service die informatie opgeslagen en integreert voor organisaties met meerdere on-premises directories en databases. U kunt het probleem met MIM-synchronisatie mogelijk oplossen als het probleem is opgelost in een recente update voor MIM of een van de andere problemen is die in de onderstaande sectie worden genoemd.

**Aanbevolen stappen**

1. Controleer of u een recente update van MIM Sync gebruikt en bekijk de opmerkingen bij de [release van MIM Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) om te bepalen of het probleem is opgelost in een update.
2. Als het probleem wordt veroorzaakt door de connector Generic LDAP, Generic SQL, Lotus Domino of Web Services, controleert u of u een recente update van de [algemene connectors gebruikt.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)
3. Als een MIM Sync-run stopt met een fout, raadpleegt u de tabel met run error [codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) om de mogelijke oorzaken te bepalen.
4. Als het uitvoeren stopt met een **uitbreidings-DLL-uitzondering,** klikt u op die woorden om het venster Eigenschappen van verbindingsruimteobject te openen en klikt u op Stapel **traceren...** voor meer informatie over de onderliggende oorzaak, zoals wordt beschreven in [Uitbreiding-DLL-Exception.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) 
5. Als het pcns-onderdeel (Password Change Notification Service) fout **6025** in het gebeurtenislogboek meldt tijdens wachtwoordsynchronisatie, raadpleegt u de handleiding voor het oplossen van problemen met [pcns-rapportagefout 6025.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)
6. Als de volledige synchronisatie met de FIM Service  Management Agent traag is, controleert u of de instelling voor automatisch groeien is vertraagd voor TempDB, zoals is beschreven in Problemen met trage of hangende volledige [synchronisatie.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)
7. Als u een fout ziet van een gestopte server met failed-creation-via-web-services met behulp van de FIM Service Management Agent, bekijkt u [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) voor een overzicht van de oorzaken.

