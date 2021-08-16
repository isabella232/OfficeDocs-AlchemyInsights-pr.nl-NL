---
title: Sitedetectie doen
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
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030753"
---
# <a name="do-site-discovery"></a>Sitedetectie doen

Als uw organisatie nog steeds oudere webtoepassingen gebruikt en van plan is de Internet Explorer-modus te gebruiken (wat de meeste klanten doen), moet u wat extra sitedetectie uitvoeren.

**U hebt al een oudere versie van een Microsoft Edge**

Als u de lijst met ondernemingssite's al hebt geconfigureerd om te werken voor de oudere versie van Microsoft Edge, is de sitedetectie bijna klaar. Het enige wat u mogelijk moet doen, is neutrale sites toevoegen.

Neutrale sites zijn meestal sites met eenmalige aanmelding (SSO). Als u naar een neutrale site gaat Microsoft Edge, wilt u in de Microsoft Edge verifiëren. Als u naar een neutrale site in de Internet Explorer-modus gaat, wilt u de internet explorer-modus gebruiken om te verifiëren.

Identificeer eenmalige aanmelding of andere neutrale sites die u gebruikt en voeg deze toe aan uw lijst met ondernemingssites.

**Internet Explorer is uw standaardbrowser**

Als u internet Explorer nu alleen gebruikt, weet u mogelijk niet welke sites zijn bijgewerkt naar moderne webstandaarden en waarvoor internet explorer nog steeds vereist is. U wilt deze sites zoeken en toevoegen aan de lijst met ondernemingssites, zodat u de internet explorer-modus alleen voor deze sites kunt gebruiken.

> [!NOTE]
> [Met Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) worden sites ontdekt die mogelijk de internet explorer-modus nodig hebben. Het kan gegevens verzamelen op computers met Windows Internet Explorer 8 tot en met Internet Explorer 11 op Windows 10, Windows 8.1 of Windows 7.

**De gegevens analyseren**

Nadat u sitegegevens hebt verzameld, raden we u het volgende proces in vier stappen aan om de gegevens te analyseren:
1. Sorteer de gegevens op domein en vervolgens op URL.
2. Definieer de grenzen van een app die u wilt configureren voor de Internet Explorer-modus. U wilt alle sites en webbesturingselementen opnemen die de app definiëren, maar u wilt geen extra sites en besturingselementen opnemen. Sommige sites kunnen net zo eenvoudig zijn als wanneer u voor andere sites of pagina's meerdere *https://contoso.com/app1* sites en pagina's moet definiëren.
3. Test de app om te controleren of deze niet inheems werkt. Veel sites bieden moderne inhoud wanneer ze een moderne browser detecteren en alleen oudere inhoud bieden wanneer ze Internet Explorer detecteren.
4. Voeg de app toe aan uw lijst met ondernemingssite als het testen mislukt.

> [!NOTE]
> Als een goede gewoonte kunt u alle sites groepen die een app bevatten. Als u een app upgradet, kunt u de hele site op deze manier gemakkelijker verwijderen uit de internet explorer-modus en een moderne browser voor die app gaan gebruiken.

Wanneer u klaar bent met sitedetectie en u de gegevens hebt geanalyseerd, kunt u uw kanaalstrategie bekijken.

