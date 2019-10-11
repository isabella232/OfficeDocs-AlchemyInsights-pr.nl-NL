---
title: Vastgelopen in outbox vanwege grote bijlagen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441301"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Berichten herstellen die vastzitten in het postvak uit

Het is raadzaam dat u begint met het uitvoeren van het scenario [' Ik heb problemen met het verzenden, ontvangen of vinden van e-mail berichten '](https://aka.ms/SaRA-OutlookSendReceive) van het hulpprogramma [Microsoft ondersteuning en herstel-assistent](https://diagnostics.office.com/#/) .

Wanneer een bericht vastloopt in het postvak uit, zijn de meest waarschijnlijke oorzaken:
- Grote bijlagen.
- De optie **direct verzenden bij verbinding** is niet ingeschakeld.

Grote bijlagen verwijderen: 

1. Selecteer in Outlook**offline werk** **verzenden/ontvangen** > . 
2. Selecteer **Postvak**uit in het navigatiedeelvenster. Vanaf hier u: 
    - Verwijder het bericht (Selecteer het en selecteer vervolgens **verwijderen**).
    - Sleep het bericht naar de map concepten, dubbelklik erop om het te openen en verwijder de bijlage Selecteer deze en selecteer vervolgens **verwijderen**).
3. Als er een foutbericht wordt weergegeven dat Outlook probeert te verzenden, sluit u Outlook. Het kan enkele ogenblikken duren om af te sluiten. Als Outlook niet wordt gesloten, drukt u op CTRL + ALT + DELETE en selecteert u **Taakbeheer starten**. Selecteer in Taakbeheer het tabblad **processen** , Scrol omlaag naar Outlook. exe en selecteer **proces beëindigen**.
4. Nadat Outlook is gesloten, start u het opnieuw en herhaalt u stap 2 en 3. 
5. Nadat u de bijlage hebt verwijderd, klikt u op**offline werk** **verzenden/ontvangen** > om online te gaan werken. 

Berichten komen ook vast te zitten in het postvak uit wanneer u op **verzenden**klikt, maar u bent niet verbonden. Klik op **verzenden/ontvangen** en Bekijk de knop **offline werken** . Als dit blauw is, wordt de verbinding verbroken. Selecteer deze om verbinding te maken (de knop wordt wit) en klik op **Alles verzenden**.
 
De optie **direct verzenden inschakelen wanneer deze is aangesloten**:
 
- Selecteer **Bestands** > **Opties** >  **Geavanceerd**.
Selecteer in de sectie **verzenden en ontvangen** de optie **direct verzenden wanneer deze is verbonden**en kies vervolgens **OK**.
 
Zie voor de volledige details:
- [Video: een vastgelopen e-mail bericht verzenden of verwijderen](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-mail blijft in de map Postvak uit totdat u handmatig een bewerking voor verzenden/ontvangen in Outlook start](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
