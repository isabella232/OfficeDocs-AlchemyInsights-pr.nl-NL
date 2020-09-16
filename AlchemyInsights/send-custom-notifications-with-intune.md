---
title: Aangepaste meldingen met intune verzenden
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720641"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Aangepaste meldingen verzenden naar de gebruikers van beheerde iOS-en Android-apparaten

Aangepaste meldingen voor intune worden verwerkt door de bedrijfs portal-app op het apparaat van een gebruiker. Vervolgens maakt de app een pushbericht op dat apparaat.

Hieronder ziet u de vereisten voor het inschakelen van de ontvangst van aangepaste meldingen en voor de app moet u vervolgens de push melding maken:

- Op het apparaat moet de bedrijfs portal-app zijn geïnstalleerd.  

- Op het toestel moet de bedrijfs portal-app pushmeldingen verzenden. Wanneer de app is geïnstalleerd of bijgewerkt, wordt de gebruiker gevraagd om meldingen toe te staan.

- Op Android-apparaten moeten Google play-services zijn geïnstalleerd.

- Het apparaat moet zijn geregistreerd met intune.

Zie de [documentatie bij de functie](https://docs.microsoft.com/intune/custom-notifications)voor meer informatie over het verzenden van een bericht.
