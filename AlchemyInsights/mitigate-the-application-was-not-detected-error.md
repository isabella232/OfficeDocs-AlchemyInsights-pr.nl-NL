---
title: Corrigeren van de fout De applicatie is niet gedetecteerd
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836346"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Corrigeren van de fout 'De applicatie is niet gedetecteerd'

De door Intune gemelde app-installatiefout 'De applicatie is niet gedetecteerd nadat de installatie is voltooid', kan optreden bij alle belangrijke besturingssystemen (Windows, iOS en Android).

De meest voorkomende scenario's die deze fout veroorzaken, zijn onder meer:

- De app is na de eerste implementatie buiten Intune bijgewerkt (vanuit een app-store van derden). Sommige toepassingen, zoals Google Chrome, voeren mogelijk automatische updates uit.
- Een gebruiker heeft de app verwijderd na de eerste installatie.

U kunt dit probleem corrigeren door eerst een revisie uit te voeren van de betrokken apparaten, om te bepalen welk scenario de fout veroorzaakt.

- Als de app is bijgewerkt buiten Intune, kunt u de app-implementatie zo instellen dat de toepassingsversie wordt genegeerd. Hiertoe stelt u onder **App-configuratie > App-informatie** de optie **App-versie negeren** in op **Ja**.
- Bij de communicatie met uw klant kan het handig zijn om de toepassing te promoten als 'vereist', om er zo voor te zorgen dat de nieuwste versie wordt geïmplementeerd.
- Het is ook mogelijk om op het iOS-platform de functionaliteit van **AutoUpdate** te gebruiken die is gekoppeld aan het Apple Volume Purchase Program. Dit kan zo worden ingesteld dat deze automatisch wordt bijgewerkt naar nieuwe toepassingsversies zodra deze beschikbaar komen.

Voor meer informatie over het oplossen van problemen met de installatie van apps, raadpleegt u [problemen met het installeren van apps.
