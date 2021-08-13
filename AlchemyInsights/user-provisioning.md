---
title: Gebruikers inrichting
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
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971334"
---
# <a name="user-provisioning"></a>Gebruikers inrichting

- Gebruik de [on-demand inrichtingsfunctie](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) om een gebruiker in te stellen en gedetailleerde diagnoses te krijgen over de stappen die zijn ondernomen.
- Zie de handleiding Voor het oplossen van problemen die u ondervindt bij het inrichten van gebruikers en groepen, de handleiding Voor probleemoplossing worden [geen gebruikers ingericht.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Zie Inrichtingslogboeken [(voorbeeld)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) in Azure Active Directory (AD) als u constateert dat gebruikers niet worden ingericht. Zoek naar logboekgegevens die betrekking hebben op een specifieke gebruiker.
- Start de inrichting regelmatig opnieuw om gebruikers te vangen die zijn gemist in een vorige inrichtingscyclus.
- De gebruiker/groep is mogelijk niet ingericht omdat onze service nog geen kans heeft gehad om de gebruiker te evalueren. Bekijk de richtlijnen voor hoe lang inrichting duurt, evenals de voortgangsbalk op de configuratiepagina voor inrichting. Als de constante status die is opgegeven in de sectie aanvullende details vóór de datum waarop de gebruiker is gemaakt/bijgewerkt/verwijderd, betekent dit dat we de gebruiker nog niet hebben geëvalueerd. In dit scenario kunt u het beste wachten totdat de inrichtingsservice is klaar. Als de constante status is bereikt, raden we u aan een herstart uit te voeren vanuit de gebruikersinterface in de Azure Portal.
  - Onze service is alleen op de hoogte van wijzigingen in een gebruiker/groep in het bronsysteem (Azure Active Directory). Als een gebruiker/groep rechtstreeks in de toepassing wordt verwijderd (bijvoorbeeld ServiceNow), zijn we niet op de hoogte van deze wijzigingen en worden deze niet terug gedraaid op basis van de status van de gebruiker in het bronsysteem. In dit scenario kunt u de wijziging het beste rechtstreeks terugdraaien in de doeltoepassing.
- Onze service heeft de gebruiker/groep geëvalueerd en heeft bepaald dat deze niet moet worden ingericht:
  - Als u het bereik hebt ingesteld op toegewezen gebruikers en groepen, controleert u of de gebruiker/groep is toegewezen aan de toepassing.
  - Als de gebruiker/groep is toegewezen aan de toepassing, controleert u of deze niet aan de standaardtoegangsrol is toegewezen. Deze rol kan niet worden gebruikt voor inrichting.
  - Als u een op kenmerken gebaseerd scoping-filter hebt ingesteld, moet u ervoor zorgen dat de gebruiker voldoet aan de criteria die u hebt opgegeven.
  - Als er al gebruikers bestaan in het doelsysteem en de status van de gebruiker in de bron- en doelmatch, zullen we geen verdere actie ondernemen.
- Onze service heeft geprobeerd de gebruiker in te stellen en deze is mislukt. Bekijk voor deze scenario's het tabblad Probleemoplossing en aanbevelingen van de inrichtingslogboeken:
  - Een vereist kenmerk van de gebruiker ontbreekt mogelijk in Azure Active Directory of komt niet overeen met de indeling die vereist is door de toepassing van derden. Het kenmerk Land van een gebruiker kan bijvoorbeeld zijn ingesteld op Verenigde Staten wanneer dit us moet zijn.
  - Het kenmerk is een referentieel kenmerk dat nog niet bestaat in de doeltoepassing. Een referentieel kenmerk is een kenmerk dat verwijst naar een ander object, bijvoorbeeld een gebruiker die lid is van een groep. De id van de gebruiker bevindt zich in het lidkenmerk van de groep, maar kan alleen worden verwerkt als het gebruikersobject waar het naar wijst al bestaat.
