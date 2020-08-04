---
title: TeamViewer gebruiken om Intune-apparaten op afstand te beheren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554972"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>TeamViewer gebruiken om Intune-apparaten op afstand te beheren

Apparaten die door Intune worden beheerd, kunnen op afstand worden beheerd met [TeamViewer.](https://www.teamviewer.com/)

Als u Intune wilt beheren met TeamViewer, voert u de volgende stappen uit: 

Begin met het verkrijgen van referenties van TeamViewer om de TeamViewer Connector op Intune in te stellen. Hierdoor kan de beheerder referenties invoeren in de Gebruikersinterface van De Verbinder van TeamViewer onder Apparaten, een eenmalige bewerking om de koppeling tussen Intune en de TeamViewer-service tot stand te brengen.

**Deel 1: Een sessie starten met een extern apparaat**

1. Selecteer onder **Alle apparaten**het apparaat waarmee u een externe sessie wilt starten.
2. Van **... Meer**, selecteer **Nieuwe hulpsessie op afstand**.
3. Selecteer **Ja** om te erkennen dat u een externe sessie wilt instellen.
    Nadat de aanvraag 'Een nieuwe externe sessie starten' is bevestigd door de TeamViewer-service, ziet u een optie om **hulp op afstand** te starten onder de details van het deelvenster Overzicht (of Essentials) voor het apparaat. Selecteer **Meer weergeven** om het deelvenster uit te vouwen en de status Hulp op afstand weer te geven.
4. Selecteer **Externe sessie starten** om de sessie aan de beheerderszijde te starten.
5. Kies ervoor om de binaire TeamViewer (Windows) te downloaden en selecteer **Uitvoeren**.<br/>
    **Opmerking** U elke webbrowserpagina negeren die is geopend voor de TeamViewer-website.

6. Bevestig het verzoek aan de TeamViewer-app om wijzigingen aan te brengen op het apparaat (alleen Windows).
7. De TeamViewer-app wordt gestart en bevat de sessiecode om de verbinding met het externe apparaat te verifiëren.

**Deel 2: Op het apparaat dat wordt gericht op een externe sessie**

1. Open het bedrijfsportaal in Intune.
2. Zoek naar een meldingsvlag: 'Uw IT-beheerder vraagt de controle over dit apparaat aan voor een hulpsessie op afstand' en selecteer de melding.
3. Kies ervoor om de TeamViewer-toepassing te downloaden of de download van de TeamViewer-app te bevestigen in de app Store en selecteer **Uitvoeren**.
    **Opmerking** U elke webbrowserpagina negeren die is geopend voor de TeamViewer-website.

4. Bevestig het verzoek aan de TeamViewer-app om wijzigingen aan te brengen op het apparaat (alleen Windows).
5. De TeamViewer-app wordt gestart en bevat de sessiecode om de verbinding met het externe apparaat te verifiëren.
6. Een pop-up vraagt of u de sessie wilt laten starten.

**Opmerking** De sessiecodes die door de TeamViewer-service worden gegenereerd, worden alleen eenmalig gebruikt. Als u de verbinding verliest, moet u:

1. Sluit de instantie van de TeamViewer-app op het externe apparaat en op het beheerwerkstation.
2. Sluit het bedrijfsportaal op het externe apparaat.
3. Start een nieuwe "Nieuwe remote Assistance session" vanuit de admin portal.
4. Open de bedrijfsportal op het externe apparaat opnieuw om de nieuwe melding te ontvangen.
5. Download en open de TeamViewer-app op zowel het externe apparaat als het beheerwerkstation, zoals voorheen.