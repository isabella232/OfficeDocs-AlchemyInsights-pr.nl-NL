---
title: Opmerkingen over lijstitems
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982452"
---
# <a name="comments-on-list-items"></a>Opmerkingen over lijstitems

Gebruikers kunnen binnenkort opmerkingen toevoegen en verwijderen van lijstitems. Gebruikers kunnen alle opmerkingen weergeven voor een item in de lijst en vervolgens filteren op andere weergaven die opmerkingen of activiteiten met betrekking tot een item weergeven.

**Tijdsinstelling** :

**Targeted release** : geleidelijke implementatie in medio oktober en verwachting met medio november

**Standard release** : geleidelijke implementatie in medio november en verwachting te voltooien vóór december

**Implementatie** : Targeted release voor de hele organisatie

Gebruikers moeten het volgende weten voordat ze opmerkingen kunnen toevoegen en verwijderen:

- Opmerkingen Volg de machtigingsinstellingen die inherent zijn in SharePoint.
- Klassieke lijsten die nog niet zijn gebouwd voor weergave in moderne gebruikersinterfaces, zoals taakoverzichten, hebben deze functie niet.
- Opmerkingen voor lijsten in teams is niet beschikbaar in deze versie.
- Opmerkingen worden niet geïndexeerd met Search.

Beheerders kunnen deze functie uitschakelen op organisatieniveau door de **CommentsOnListItemsDisabled** -parameter in de PowerShell **-cmdlet Set-SPOTenant** te wijzigen.

Het is op dit moment niet mogelijk om opmerkingen in te schakelen op de site of het lijstniveau. We hopen dat deze besturingselementen in een latere update liggen, waarschijnlijk in het eerste kwartaal 2021.
