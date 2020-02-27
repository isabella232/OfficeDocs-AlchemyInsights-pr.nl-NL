---
title: Maak een e-mailvangst allemaal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286105"
---
# <a name="create-an-email-catch-all"></a>Maak een e-mailvangst allemaal

Het gebruik van een vangst wordt sterk afgeraden. Het is beter om een bounce terug te geven aan de afzender om afzenders te laten weten dat hun bericht niet kan worden bezorgd zoals geadresseerd, zodat ze actie kunnen ondernemen. U het bewaakte postvak ook beperken tot alleen voorheen geldige e-mailadressen. 

Elke vangst alle mailbox ontvangt een groot deel van spam en kan uiteindelijk vullen, indien niet nauwlettend gecontroleerd. (Er zijn ontvangstlimieten.) 

Als u besluit door te gaan, voert u de volgende stappen uit:

1. Maak een dynamische distributiegroep & 'Alle typen geadresseerden' bevatten.

2. Maak een speciaal postvak om bijvoorbeeld e-mails te vangen catchall@domain.com.

3. Stel voor het specifieke domein het DomainType in op "InternalRelay". Als u later de vangst allemaal verwijdert, moet u het domein terugzetten naar Authoritative.

4. Maak als volgt een mailflow-transportregel:

    - Als de afzender 'Buiten de organisatie' staat
    - Het bericht omleiden naar Catchall@domain.com
    - Behalve als de ontvanger lid is van allusers@domain.com (Distributiegroep bevat alle leden)
    - Ervoor zorgen dat nieuwe postvakken worden toegevoegd aan de dynamische distributiegroep
