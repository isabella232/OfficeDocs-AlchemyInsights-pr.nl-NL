---
title: Inrichting door gebruiker
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
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481362"
---
# <a name="user-provisioning"></a>Inrichting door gebruiker

- Gebruik de [on-demand inrichtingsmogelijkheid](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) om een gebruiker in terichten en gedetailleerde diagnostische gegevens te krijgen over de ondernomen stappen.
- Zie de handleiding Voor het oplossen van problemen die u ondervindt bij het inrichten van gebruikers en groepen, de handleiding Geen gebruikers [worden ingericht.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Zie Inrichtingslogboeken [(preview)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) in Azure Active Directory (AD) als u ziet dat gebruikers niet worden ingericht. Zoek naar logboekgegevens die betrekking hebben op een specifieke gebruiker.
- De inrichting van de inrichting regelmatig opnieuw starten om alle gebruikers te zien die in een vorige inrichtingscyclus zijn gemist.
- De gebruiker/groep is mogelijk niet ingericht omdat onze service de gebruiker nog niet heeft kunnen evalueren. Bekijk de richtlijnen voor de tijd die nodig is voor de inrichting en voor de voortgangsbalk op de configuratiepagina voor inrichting. Als de constante status die is opgegeven in de sectie met aanvullende gegevens vóór de datum valt waarop de gebruiker is gemaakt/bijgewerkt/verwijderd, betekent dit dat de gebruiker nog niet is geëvalueerd. In dit scenario kunt u het beste wachten totdat de inrichtingsservice is voltooien. Als de constante status is bereikt, raden we u aan een herstart uit de gebruikersinterface in de Azure Portal uit te voeren.
  - Onze service is alleen op de hoogte van wijzigingen in een gebruiker/groep in het bronsysteem (Azure Active Directory). Als een gebruiker/groep rechtstreeks in de toepassing is verwijderd (bijvoorbeeld ServiceNow), zijn we niet op de hoogte van deze wijzigingen en draaien we deze niet terug op basis van de status van de gebruiker in het bronsysteem. In dit scenario kunt u de wijziging het beste rechtstreeks terugdraaien in de doeltoepassing.
- Onze service heeft de gebruiker/groep geëvalueerd en heeft vastgesteld dat deze niet moet worden ingericht:
  - Als u het bereik hebt ingesteld op toegewezen gebruikers en groepen, controleert u of de gebruiker/groep is toegewezen aan de toepassing.
  - Als de gebruiker/groep aan de toepassing is toegewezen, controleert u of deze niet zijn toegewezen aan de standaardtoegangsrol. Deze rol kan niet worden gebruikt voor de inrichting.
  - Als u een op een kenmerk gebaseerd bereikfilter hebt ingesteld, controleert u of de gebruiker voldoet aan de criteria die u hebt opgegeven.
  - Als er al gebruikers in het doelsysteem aanwezig zijn en de status van de gebruiker in de bron- en doel-overeenkomst, worden er geen verdere acties ondernomen.
- Onze service heeft geprobeerd de gebruiker in te leveren en deze is mislukt. Voor deze scenario's bekijkt u het tabblad Probleemoplossing en aanbevelingen van de inrichtingslogboeken:
  - Een vereist kenmerk van de gebruiker ontbreekt mogelijk in Azure Active Directory of komt niet overeen met de indeling die vereist is voor de toepassing van derden. Het kenmerk Land van een gebruiker kan bijvoorbeeld zijn ingesteld op Verenigde Staten, terwijl dat VS moet zijn.
  - Het kenmerk is een referentaal kenmerk dat nog niet aanwezig is in de doeltoepassing. Een referentiële kenmerk is een kenmerk dat verwijst naar een ander object, bijvoorbeeld een gebruiker die lid is van een groep. De id van de gebruiker bevindt zich in het lidkenmerk van de groep, maar kan alleen worden verwerkt als het gebruikersobject waar het object naar wijst al bestaat.
