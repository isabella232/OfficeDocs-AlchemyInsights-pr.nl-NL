---
title: Probleem met kenmerk en bereikfilter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481363"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Probleem met kenmerk en bereikfilter

**Probleem met conflicterende UPN-waarden**

Op de werkdag naar AD User Provisioning Workday to AD User Provisioning wordt het foutbericht **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique weergegeven.** De bewerking is mislukt omdat de UPN-waarde voor toevoeging/wijziging niet uniek is voor het hele bos. Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.

De **userPrincipalName-waarde** die de Werkdag-connector probeert in te stellen bij het maken van het AD-gebruikersaccount bestaat al in het doel-AD-domein. Dit houdt in dat ofwel (1) de gebruiker al bestaat en dat de bijbehorende id-controle is mislukt voor de gebruiker of (2) de UPN-generatieregel een conflicterende waarde genereert.

Hier volgen de voorgestelde stappen voor een oplossing:

Als het werkdagaccount niet kan worden gekoppeld aan het Active Directory-account door de overeenkomende id-controle, controleert u of het overeenkomende id-kenmerk (meestal werknemer-id) in zowel Werkdag als AD een exacte overeenkomst heeft. Als ze geen overeenkomst hebben, is het een gegevensprobleem dat moet worden opgelost. Als de werknemer-id op werkdag bijvoorbeeld 001052 is en in AD 1052, dan worden de twee accounts niet gekoppeld met de inrichtingsen engine en wordt geprobeerd een gebruiker te maken die al bestaat. In dit geval kunt u de waarde **EmployeeID** in AD wijzigen om de voorvoeglijke nullen op te nemen, waardoor deze 001052 wordt.
Als de UPN-genererende expressie geen unieke waarde genereert, kunt u overwegen om de functie De duplicatie **SelectUniqueValue** te gebruiken om elke keer een unieke waarde te genereren.

**Werkdag naar AD User Provisioning stelt geen kenmerkwaarde voor manager in voor AD-gebruikersaccount**

Met de taak Werkdag naar AD-gebruikers inrichting wordt de kenmerkwaarde van het **managerkenmerk** niet voor AD-gebruikersaccounts instelling. Er zijn twee scenario's mogelijk waarin dit gedrag wordt gezien:

1. De manager in werkdag kan niet worden opgelost met een bijbehorend ad-gebruikersaccount omdat de manager niet binnen het bereik valt.
2. In een **scenario met meerdere AD-domeinen** is de manager in werkdag niet aanwezig in hetzelfde domein als de gebruiker.

Probeer de volgende stappen om het probleem op te lossen:

1. Als u bereikfilters hebt gedefinieerd, controleert u eerst of de manager binnen het bereik valt en of de scoping-component wordt gebruikt. Als de manager niet voldoet aan het bereikfilter, wijzigt u het filter zodat de manager ook binnen het bereik van de inrichtingsbewerking valt.
2. Als u meerdere AD-domeinen hebt, geldt voor de connector een bekende beperking dat het niet mogelijk is om verwijzingen naar domeinbeheer op te lossen.

Zie Zelfstudie: Werkdag configureren voor het automatisch inrichten van gebruikers voor meer informatie over het configureren van de werkdag voor automatische [inrichting.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)













