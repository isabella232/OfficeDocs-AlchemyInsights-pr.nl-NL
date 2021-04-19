---
title: Windows Memory Diagnostics uitvoeren in Windows 10
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826662"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Windows Memory Diagnostics uitvoeren in Windows 10

Als Windows en apps op uw pc crashen, vastvriezen of instabiel werken, hebt u mogelijk een probleem met het geheugen (RAM) van de pc. U kunt de Windows Memory Diagnostic uitvoeren om te controleren op problemen met het RAM-geheugen van de pc.

Typ in het zoekvak op de taakbalk **geheugendiagnose** en selecteer **vervolgens Windows Memory Diagnostic**. 

Als u de diagnose wilt uitvoeren, moet de pc opnieuw worden gestart. U hebt de optie om direct opnieuw te starten (sla uw werk op en sluit eerst documenten en e-mailberichten) of plan de diagnostische test automatisch uit te voeren wanneer de pc de volgende keer opnieuw wordt gestart:

![Windows Memory Diagnostic](media/windows-memory-diagnostic.png)

Wanneer de pc opnieuw wordt gestart, wordt het **Windows Memory Diagnostics Tool** automatisch uitgevoerd. Status en voortgang worden weergegeven terwijl de diagnostische gegevens worden uitgevoerd en u kunt de diagnostische gegevens annuleren door op de **ESC-toets** op het toetsenbord te drukken.

Wanneer de diagnostische gegevens zijn voltooid, start Windows normaal.
Direct na het opnieuw opstarten, wanneer het bureaublad wordt  weergegeven, wordt er een melding weergegeven (naast het pictogram Actiecentrum op de taakbalk) om aan te geven of er geheugenfouten zijn gevonden. Bijvoorbeeld:

Hier ziet u het pictogram Actiecentrum: ![Pictogram Actiecentrum](media/action-center-icon.png) 

En een voorbeeldmelding: ![Geen geheugenfouten](media/no-memory-errors.png)

Als u de melding hebt  gemist, kunt u het pictogram Actiecentrum op de taakbalk selecteren om het **Actiecentrum** weer te geven en een schuifbare lijst met meldingen te zien.

Als u gedetailleerde informatie wilt bekijken, **typt u gebeurtenis** in het zoekvak op de taakbalk en selecteert u **Gebeurtenisviewer**. Ga in **het linkerdeelvenster** van eventviewer naar **Windows Logs > System.** Scan in het rechterdeelvenster de lijst terwijl  u naar de kolom Bron kijkt, totdat u gebeurtenissen ziet met Bronwaarde **MemoryDiagnostics-Results**. Markeer elke dergelijke gebeurtenis en bekijk de resultaatgegevens in het vak onder **het** tabblad Algemeen onder de lijst.
