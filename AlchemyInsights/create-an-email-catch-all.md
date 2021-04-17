---
title: Een e-mail catch all maken
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816195"
---
# <a name="create-an-email-catch-all"></a>Een e-mail catch all maken

Het gebruik van een catch all wordt sterk afgeraden. Het is beter om een bounce terug te geven aan de afzender om afzenders te laten weten dat hun bericht niet kan worden bezorgd als geadresseerd, zodat ze actie kunnen ondernemen. U kunt het bewaakte postvak ook beperken tot alleen voorheen geldige e-mailadressen. 

Elke catch all mailbox ontvangt een groot deel van de spam en kan uiteindelijk worden gevuld als het niet goed wordt gecontroleerd. (Er zijn ontvangstlimieten.) 

Als u besluit verder te gaan, volgt u de volgende stappen:

1. Maak een dynamische distributiegroep & 'Alle typen geadresseerden'.

2. Maak een speciaal postvak om e-mailberichten te ontvangen, bijvoorbeeld catchall@domain.com.

3. Stel voor het specifieke domein het DomainType in op 'InternalRelay'. Als u de catch all later verwijdert, moet u het domein opnieuw instellen op Gezaghebbend.

4. Maak als volgt een Mailflow-transportregel:

    - Als de afzender 'Buiten de organisatie' is
    - Het bericht omleiden naar Catchall@domain.com
    - Behalve als de geadresseerde lid is van allusers@domain.com (Distributiegroep bevat alle leden)
    - Controleer of nieuwe postvakken worden toegevoegd aan de dynamische distributiegroep
