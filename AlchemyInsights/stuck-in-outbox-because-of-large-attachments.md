---
title: Stuck in Outbox vanwege grote bijlagen
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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241247"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Berichten herstellen die vastzitten in het postvak uit

We raden u aan eerst het scenario ['Ik heb problemen met het verzenden, ontvangen of vinden van e-mailberichten'](https://aka.ms/SaRA-OutlookSendReceive) uit te voeren vanuit het hulpprogramma [Microsoft Support and Recovery Assistant.](https://diagnostics.office.com/#/)

Wanneer een bericht vast komt te zitten in uw postvak IN, is de meest waarschijnlijke oorzaak een grote bijlage of is de optie 'Onmiddellijk verzenden wanneer verbonden' niet ingeschakeld.

**De grote bijlage verwijderen**

1. Selecteer in Outlook **Offline verzenden / Ontvangen** > **van werk**. 
2. Selecteer **Uitvak**in het navigatiedeelvenster . Vanaf hier u: 
    - Verwijder het bericht (selecteer het bericht en selecteer **Verwijderen).**
    - Sleep het bericht naar de map Concepten, dubbelklik om het te openen en verwijder de bijlage selecteer het bericht en selecteer **Verwijderen**).
3. Als u een fout ontvangt waarin staat dat Outlook probeert het bericht te verzenden, sluit u Outlook. Het kan even duren voordat je het afgaat. Als Outlook niet wordt gesloten, drukt u op Ctrl+Alt+Verwijderen en selecteert **u Taakbeheer starten**. Selecteer in Taakbeheer het tabblad **Processen,** scrol omlaag naar outlook.exe en selecteer **Proces beëindigen**.
4. Nadat Outlook is gesloten, start u het opnieuw op en herhaalt u stap 2 en 3. 
5. Nadat u de bijlage hebt verwijderd, klikt u op Werk verzenden **/ ontvangen** > **offline** om verder te werken online. 

Berichten komen ook vast te zitten in het postvak UIT wanneer u op **Verzenden**klikt, maar u bent niet verbonden. Klik **op Verzenden / Ontvangen** en kijk op de knop Offline **werken.** Als het blauw is, wordt de verbinding verbroken. Klik erop om verbinding te maken (de knop wordt wit) en klik op **Alles verzenden**.
 
**Verzenden onmiddellijk inschakelen wanneer deze is aangesloten**
 
1. Klik op het tabblad Bestand op **Opties**.

2. Klik in het dialoogvenster Outlook-opties op **Geavanceerd**.

3. Klik in de sectie Verzenden en ontvangen om verzenden onmiddellijk in te schakelen **wanneer deze is verbonden.** Klik op **OK**.
 
Zie voor meer informatie:
- [Video: Een vastgelopen e-mail verzenden of verwijderen](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-mail blijft in de map Outbox totdat u handmatig een verzend-/ontvangstbewerking in Outlook start](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
