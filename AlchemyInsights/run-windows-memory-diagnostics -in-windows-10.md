---
title: Windows-geheugendiagnose uitvoeren in Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289759"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Windows-geheugendiagnose uitvoeren in Windows 10

Als Windows en apps op uw pc crashen, bevriezen of op een instabiele manier werken, hebt u mogelijk een probleem met het geheugen (RAM) van de pc. U de Windows Memory Diagnostic uitvoeren om te controleren op problemen met het RAM-geheugen van de pc.

Typ in het zoekvak op de taakbalk **geheugendiagnose**en selecteer **Vervolgens Windows Memory Diagnostic**. 

Als u de diagnose wilt uitvoeren, moet de pc opnieuw worden opgestart. U hebt de mogelijkheid om onmiddellijk opnieuw op te starten (sla uw werk op en sluit eerst geopende documenten en e-mails), of plan de diagnose automatisch uit te voeren wanneer de pc de volgende keer opnieuw wordt opgestart:

![Windows-geheugendiagnose](media/windows-memory-diagnostic.png)

Wanneer de pc opnieuw wordt opgestart, wordt het **Windows Memory Diagnostics Tool** automatisch uitgevoerd. Status en voortgang worden weergegeven als de diagnostische uitvoering en u hebt de mogelijkheid om de diagnose te annuleren door op de **ESC-toets** op uw toetsenbord te drukken.

Wanneer de diagnose is voltooid, wordt Windows normaal gestart.
Onmiddellijk na het opnieuw opstarten, wanneer het bureaublad wordt weergegeven, verschijnt er een melding (naast het pictogram **Van het Onderhoudscentrum** op de taakbalk), om aan te geven of er geheugenfouten zijn gevonden. Bijvoorbeeld:

Hier is het pictogram Actiecentrum: ![Pictogram Actiecentrum](media/action-center-icon.png) 

En een voorbeeldmelding: ![Geen geheugenfouten](media/no-memory-errors.png)

Als u de melding hebt gemist, u het pictogram **Onderhoudscentrum** op de taakbalk selecteren om het **Onderhoudscentrum** weer te geven en een schuifbare lijst met meldingen te bekijken.

Als u gedetailleerde informatie wilt bekijken, typt u **een gebeurtenis** in het zoekvak op de taakbalk en selecteert u **Logboeken**. Navigeer in het linkerdeelvenster van **logboeken**naar **Windows Logs > System.** Scan in het rechterdeelvenster de lijst terwijl u naar de kolom **Bron** kijkt, totdat u gebeurtenissen ziet met **Bronwaarde MemoryDiagnostics-Results**. Markeer elke gebeurtenis en zie de resultaatinformatie in het vak onder het tabblad **Algemeen** onder de lijst.
