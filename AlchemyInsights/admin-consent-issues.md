---
title: Problemen met beheerders instemming
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
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900929"
---
# <a name="admin-consent-issues"></a>Problemen met beheerders instemming

1. Schakel de [beheerder toestemming](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) voor het doorgeven van beheerders rechtstreeks vanuit het scherm voor toestemming in.

1. Zie het volgende artikel voor de stappen voor probleemoplossing: [onverwachte fout bij het uitvoeren van een aanvraag voor](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)het oplossen van problemen wanneer gebruikers van de toepassing onverwachte fouten zien tijdens het toestemming proces.

1. Meer informatie over [beheerders aanvragen voor het Microsoft-identiteits platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), de werking van de [instemming](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) en de [beoordeling van een aanvraag voor de beheerders vergunning voor de gehele Tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Toepassingen die worden geïntegreerd met Microsoft Identity platform volgen een machtigings model waarmee gebruikers en beheerders kunnen bepalen hoe gegevens kunnen worden geopend. De implementatie van het autorisatie model op het Microsoft Identity platform-eindpunt is bijgewerkt en de manier waarop een app moet communiceren met het Microsoft-identiteits platform. Zie [machtigingen en instemming in het eindpunt van Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) voor een overzicht van dit autorisatie model, waaronder bereiken, machtigingen en toestemming.