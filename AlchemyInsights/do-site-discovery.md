---
title: Sitedetectie
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692936"
---
# <a name="do-site-discovery"></a>Sitedetectie

Als uw organisatie nog steeds gebruikmaakt van oudere webtoepassingen en abonnementen voor het gebruik van de Internet Explorer-modus (wat de meeste klanten doen), moet u aanvullende sitedetectie uitvoeren.

**U hebt al een oudere versie van Microsoft Edge geïmplementeerd**

Als u de lijst met ondernemingssite's al hebt geconfigureerd voor de oudere versie van Microsoft Edge, is uw sitedetectie bijna klaar. Het enige wat u mogelijk moet doen, is het toevoegen van neutrale sites.

Neutrale sites zijn meestal sites die eenmalige aanmelding bieden. Als u vanuit Microsoft Edge naar een neutrale site gaat, wilt u in Microsoft Edge blijven voor verificatie. Als u naar een neutrale site gaat in de Internet Explorer-modus, wilt u in de Internet Explorer-modus blijven voor verificatie.

Identificeer eenmalige aanmelding of andere neutrale sites die u gebruikt en voeg deze toe aan uw lijst met ondernemingssites.

**Internet Explorer is uw standaardbrowser**

Als u nu alleen Internet Explorer gebruikt, weet u mogelijk niet welke sites zijn bijgewerkt naar moderne webstandaards en voor welke sites Internet Explorer nog steeds is vereist. U zult deze sites willen zoeken en toevoegen aan de lijst met ondernemingssites, zodat u de Internet Explorer-modus alleen voor deze sites kunt gebruiken.

> [!NOTE]
> [Met Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) worden sites gevonden die mogelijk de Internet Explorer-modus nodig hebben. Het kan gegevens verzamelen op computers met Windows Internet Explorer 8 tot en met Internet Explorer 11 op Windows 10, Windows 8.1 of Windows 7.

**De gegevens analyseren**

Nadat u sitegegevens hebt verzameld, wordt u aangeraden de volgende vier stappen uit te zetten om de gegevens te analyseren:
1. Sorteer de gegevens op domein en vervolgens op URL.
2. Definieer de grenzen van een app die u wilt configureren voor de Internet Explorer-modus. U wilt alle sites en webbesturingselementen opnemen die de app definiëren, maar u wilt geen extra sites en besturingselementen opnemen. Sommige sites zijn zo eenvoudig als terwijl u voor andere sites meerdere sites en *https://contoso.com/app1* pagina's moet definiëren.
3. Test de app om te controleren of deze niet in het eigen land werkt. Veel sites bieden moderne inhoud wanneer ze een moderne browser detecteren en bieden alleen verouderde inhoud wanneer Internet Explorer wordt gedetecteerd.
4. Voeg de app toe aan de lijst met ondernemingssite's als het testen mislukt.

> [!NOTE]
> U wordt daarom het beste alle sites in een app gegroepeerd. Wanneer u een app upgradet, is het dan eenvoudiger om de hele site uit de Internet Explorer-modus te verwijderen en een moderne browser voor die app te gebruiken.

Wanneer u klaar bent met sitedetectie en de gegevens hebt geanalyseerd, kunt u uw kanaalstrategie bekijken.

