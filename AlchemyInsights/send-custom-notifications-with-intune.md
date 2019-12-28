---
title: Aangepaste meldingen verzenden met intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886852"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Aangepaste meldingen verzenden naar gebruikers van beheerde iOS-en Android-apparaten

Aangepaste meldingen voor intune worden verwerkt door de bedrijfs portal-app op het apparaat van een gebruiker. De app maakt vervolgens de pushmelding op dat apparaat.

De volgende zijn apparaatvereisten ter ondersteuning van de ontvangst van aangepaste meldingen en voor de app vervolgens de pushmelding maken:

- Het apparaat moet de bedrijfs portal-app hebben geïnstalleerd.  

- Het apparaat moet de bedrijfs portal-app toestaan om pushmeldingen te verzenden. Wanneer de app is geïnstalleerd of bijgewerkt, wordt de gebruiker gevraagd om meldingen toe te staan.

- Op Android-apparaten moeten Google play-services zijn geïnstalleerd.

- Het apparaat moet zijn geregistreerd bij intune.

Zie de documentatie bij de [functie](https://docs.microsoft.com/intune/custom-notifications)voor meer informatie, zoals het verzenden van een bericht.
