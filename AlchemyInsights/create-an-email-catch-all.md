---
title: Maak een e-mail-catch all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712981"
---
# <a name="create-an-email-catch-all"></a>Maak een e-mail-catch all

Het gebruik van een catch-all wordt sterk ontmoedigd. Het is beter om de afzender te laten weten dat ze hun bericht niet kunnen afleveren als geadresseerd zodat ze een actie kunnen ondernemen. U kunt ook het bewaakte postvak beperken, zodat alleen eerder geldige e-mailadressen worden onderschept. 

Willekeurige vangst berichten ontvangen een goede aanbieding van spam en kunnen uiteindelijk opvullen, indien niet nauwkeurig wordt gecontroleerd. (Er worden limieten ontvangen.) 

Als u wilt doorgaan, gaat u als volgt te werk:

1. Maak een dynamische distributiegroep & Neem de ' alle typen geadresseerden '.

2. Maak een specifiek postvak voor het verwerken van e-mailberichten, bijvoorbeeld catchall@domain.com.

3. Stel voor het specifieke domein de DomainType in op ' InternalRelay '. Als u de optie catch later verwijdert, dient u het domein weer in te stellen op gezaghebbend.

4. Maak als volgt een transport-Transport regel:

    - Als de afzender zich buiten de organisatie bevindt
    - Het bericht omleiden naar Catchall@domain.com
    - Behalve als de ontvanger lid is van allusers@domain.com (distributiegroep bevat alle leden)
    - Controleren of nieuwe postvakken worden toegevoegd aan de dynamische distributiegroep
