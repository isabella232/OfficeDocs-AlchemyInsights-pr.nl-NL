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
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429716"
---
# <a name="problem-with-single-user"></a>Probleem met één gebruiker

- De gebruiker is mogelijk niet ingericht omdat de service de gebruiker nog niet heeft kunnen evalueren. Bekijk de richtlijnen voor de tijd die nodig is voor de inrichting en voor de voortgangsbalk op de configuratiepagina voor inrichting. Als de constante status die is opgegeven in de sectie met aanvullende gegevens vóór de datum valt waarop de gebruiker is gemaakt/bijgewerkt/verwijderd, betekent dit dat de gebruiker nog niet is geëvalueerd. In dit scenario kunt u het beste wachten totdat de inrichtingsservice is voltooien.

  - Onze service is alleen op de hoogte van wijzigingen voor een gebruiker in het bronsysteem (Cloud HR). Er moet een geldige wijziging zijn in het bronsysteem voor Azure AD om de wijziging te detecteren en deze door te stromen naar Active Directory.
- De inrichtingsservice heeft de gebruiker geëvalueerd en vastgesteld dat deze niet moet worden ingericht:
  - Als u een op een kenmerk gebaseerd bereikfilter hebt ingesteld, controleert u of de gebruiker voldoet aan de criteria die u hebt opgegeven.
  - Als er al gebruikers in het doelsysteem aanwezig zijn en de status van de gebruiker in de bron- en doel-overeenkomst, worden er geen verdere acties ondernomen.
- Er is een poging ondernomen om de gebruiker in te inrichting. De inrichtingsservice is mislukt. Voor deze scenario's bekijkt u het tabblad Probleemoplossing en aanbevelingen van de inrichtingslogboeken:
  - Een vereist kenmerk van de gebruiker ontbreekt mogelijk in on-premises Active Directory of Azure AD. De regels userPrincipalName of sAMAccountName genereren bijvoorbeeld niet de juiste waarde.
  - Het overeenkomende kenmerk (meestal employeeId) kan niet worden opgelost voor een unieke gebruiker in on-premises Active Directory of Azure AD. Er zijn bijvoorbeeld twee gebruikers met dezelfde employeeId in AD en de service retourneert een foutcode die dubbele doelgegevens aangeeft voor dezelfde broninvoer.

Zie De inrichtingslogboeken voor een probleem met een specifieke gebruiker bekijken als u logboeken voor één gebruiker en groepen [wilt bekijken.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
