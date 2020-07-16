---
title: Problemen met het openen of downloaden van bestanden in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148249"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problemen met het openen of downloaden van bestanden in Yammer

Classic Yammer ondersteunt meerdere opties voor bestandsuploads naar berichten en groepen. Afhankelijk van de netwerkconfiguratie worden bestanden standaard opgeslagen in SharePoint.

De bestandenkiezer in de nieuwe Yammer biedt nog niet alle opties die beschikbaar zijn in de klassieke Yammer. Een toekomstige update voegt extra functies toe. Zie [Een bestand of afbeelding toevoegen aan een Yammer-gespreksbericht voor](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)meer informatie.

**Kan een bestand niet openen of downloaden**  

Een bestand kan worden geüpload naar Yammer, maar ook een koppeling naar een bestand in SharePoint Online. Als u problemen wilt oplossen, moet u eerst de locatie van het bestand bepalen. Als het bestand is geüpload naar Yammer, heeft het een URL van *.yammer.com. Controleer of de vereiste URL's en IP-adressen worden gedeblokkeerd. Zie voor meer informatie het blogbericht [Het gebruik van hardgecodeerde IP-adressen voor Yammer wordt niet aanbevolen.](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)

Controleer of een gebruiker die ook een globale beheerder is, het bestand kan downloaden. Als het bestand privé is, moet u mogelijk de modus Privé-inhoud gebruiken. Zie [Privé-inhoud bewaken in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)voor meer informatie.  

**Gasten en bestanden op Yammer-netwerkniveau in SharePoint Online**  

[Gasten op netwerkniveau in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) gebruiken Azure AD B2B niet en zijn intern voor de Yammer-service, zodat ze geen toegang hebben tot Yammer-bestanden die zijn opgeslagen in SharePoint. Maak een externe AAD B2B-gebruiker die met die identiteit toegang heeft tot documentbibliotheken in SharePoint Online. Zie Ondersteuning voor ondersteuning voor gasten [in Yammer in Yammer voor](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)meer informatie over toekomstige Azure AD B2B-gastondersteuning in Yammer.