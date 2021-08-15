---
title: Probleem met één gebruiker
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960146"
---
# <a name="problem-with-single-user"></a>Probleem met één gebruiker

- De gebruiker is mogelijk niet ingericht omdat de service nog geen kans heeft gehad om de gebruiker te evalueren. Bekijk de richtlijnen voor hoe lang inrichting duurt, evenals de voortgangsbalk op de configuratiepagina voor inrichting. Als de constante status die is opgegeven in de sectie aanvullende details vóór de datum waarop de gebruiker is gemaakt/bijgewerkt/verwijderd, betekent dit dat we de gebruiker nog niet hebben geëvalueerd. In dit scenario kunt u het beste wachten totdat de inrichtingsservice is klaar.

  - Houd er rekening mee dat onze service alleen op de hoogte is van wijzigingen in een gebruiker in het bronsysteem (Cloud HR). Er moet een geldige wijziging zijn in het bronsysteem voor Azure AD om de wijziging te detecteren en door te stromen naar Active Directory.
- De inrichtingsservice heeft de gebruiker geëvalueerd en heeft bepaald dat deze niet moet worden ingericht:
  - Als u een op kenmerken gebaseerd scoping-filter hebt ingesteld, moet u ervoor zorgen dat de gebruiker voldoet aan de criteria die u hebt opgegeven.
  - Als er al gebruikers bestaan in het doelsysteem en de status van de gebruiker in de bron- en doelmatch, zullen we geen verdere actie ondernemen.
- De inrichtingsservice heeft geprobeerd de gebruiker in te stellen en deze is mislukt. Bekijk voor deze scenario's het tabblad Probleemoplossing en aanbevelingen van de inrichtingslogboeken:
  - Mogelijk ontbreekt er een vereist kenmerk voor de gebruiker in on-premises Active Directory of Azure AD. De generatieregels userPrincipalName of sAMAccountName genereren bijvoorbeeld niet de juiste waarde.
  - Het overeenkomende kenmerk (meestal employeeId) wordt niet opgelost voor een unieke gebruiker in on-premises Active Directory of Azure AD. Er zijn bijvoorbeeld twee gebruikers met dezelfde employeeId in AD en de service retourneert een foutcode die dubbele doelgegevens aangeeft voor dezelfde broninvoer.

Zie De inrichtingslogboeken controleren voor een probleem met een specifieke gebruiker als u logboeken voor één gebruiker en groepen [wilt bekijken.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
