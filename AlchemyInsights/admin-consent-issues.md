---
title: Problemen met toestemming van beheerder
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952568"
---
# <a name="admin-consent-issues"></a>Problemen met toestemming van beheerder

1. Schakel de [werkstroom voor beheerdersmachtiging](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) in om gebruikers toe te staan om goedkeuring van de beheerder rechtstreeks vanuit het toestemmingsscherm aan te vragen.

1. Als u of de gebruikers van uw toepassing onverwachte fouten zien tijdens het toestemmingsproces, bekijkt u dit artikel voor het oplossen van stappen: Onverwachte fout bij het uitvoeren van toestemming voor [een toepassing.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Meer informatie over toestemming van beheerders voor [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) [Microsoft identity platform,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)hoe de toestemmingsprompt werkt en hoe u een aanvraag voor toestemming voor beheerders voor de hele tenant [evalueert.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Toepassingen die met een Microsoft identity platform worden geïntegreerd, volgen een autorisatiemodel dat gebruikers en beheerders controle geeft over hoe gegevens kunnen worden gebruikt. De implementatie van het autorisatiemodel is bijgewerkt op het Microsoft identity platform eindpunt en de manier waarop een app moet werken met de Microsoft identity platform. Zie Machtigingen en toestemming in het Microsoft identity platform eindpunt voor een overzicht van dit autorisatiemodel, inclusief [scopes,](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) machtigingen en toestemming.