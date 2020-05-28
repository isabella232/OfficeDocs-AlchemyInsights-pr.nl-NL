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
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="77860-102">Windows-geheugendiagnose uitvoeren in Windows 10</span><span class="sxs-lookup"><span data-stu-id="77860-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="77860-103">Als Windows en apps op uw pc crashen, bevriezen of op een instabiele manier werken, hebt u mogelijk een probleem met het geheugen (RAM) van de pc.</span><span class="sxs-lookup"><span data-stu-id="77860-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="77860-104">U de Windows Memory Diagnostic uitvoeren om te controleren op problemen met het RAM-geheugen van de pc.</span><span class="sxs-lookup"><span data-stu-id="77860-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="77860-105">Typ in het zoekvak op de taakbalk **geheugendiagnose**en selecteer **Vervolgens Windows Memory Diagnostic**.</span><span class="sxs-lookup"><span data-stu-id="77860-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="77860-106">Als u de diagnose wilt uitvoeren, moet de pc opnieuw worden opgestart.</span><span class="sxs-lookup"><span data-stu-id="77860-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="77860-107">U hebt de mogelijkheid om onmiddellijk opnieuw op te starten (sla uw werk op en sluit eerst geopende documenten en e-mails), of plan de diagnose automatisch uit te voeren wanneer de pc de volgende keer opnieuw wordt opgestart:</span><span class="sxs-lookup"><span data-stu-id="77860-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows-geheugendiagnose](media/windows-memory-diagnostic.png)

<span data-ttu-id="77860-109">Wanneer de pc opnieuw wordt opgestart, wordt het **Windows Memory Diagnostics Tool** automatisch uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="77860-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="77860-110">Status en voortgang worden weergegeven als de diagnostische uitvoering en u hebt de mogelijkheid om de diagnose te annuleren door op de **ESC-toets** op uw toetsenbord te drukken.</span><span class="sxs-lookup"><span data-stu-id="77860-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="77860-111">Wanneer de diagnose is voltooid, wordt Windows normaal gestart.</span><span class="sxs-lookup"><span data-stu-id="77860-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="77860-112">Onmiddellijk na het opnieuw opstarten, wanneer het bureaublad wordt weergegeven, verschijnt er een melding (naast het pictogram **Van het Onderhoudscentrum** op de taakbalk), om aan te geven of er geheugenfouten zijn gevonden.</span><span class="sxs-lookup"><span data-stu-id="77860-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="77860-113">Bijvoorbeeld:</span><span class="sxs-lookup"><span data-stu-id="77860-113">For example:</span></span>

<span data-ttu-id="77860-114">Hier is het pictogram Actiecentrum:</span><span class="sxs-lookup"><span data-stu-id="77860-114">Here's the Action Center icon:</span></span> ![Pictogram Actiecentrum](media/action-center-icon.png) 

<span data-ttu-id="77860-116">En een voorbeeldmelding:</span><span class="sxs-lookup"><span data-stu-id="77860-116">And a sample notification:</span></span> ![Geen geheugenfouten](media/no-memory-errors.png)

<span data-ttu-id="77860-118">Als u de melding hebt gemist, u het pictogram **Onderhoudscentrum** op de taakbalk selecteren om het **Onderhoudscentrum** weer te geven en een schuifbare lijst met meldingen te bekijken.</span><span class="sxs-lookup"><span data-stu-id="77860-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="77860-119">Als u gedetailleerde informatie wilt bekijken, typt u **een gebeurtenis** in het zoekvak op de taakbalk en selecteert u **Logboeken**.</span><span class="sxs-lookup"><span data-stu-id="77860-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="77860-120">Navigeer in het linkerdeelvenster van **logboeken**naar **Windows Logs > System.**</span><span class="sxs-lookup"><span data-stu-id="77860-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="77860-121">Scan in het rechterdeelvenster de lijst terwijl u naar de kolom **Bron** kijkt, totdat u gebeurtenissen ziet met **Bronwaarde MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="77860-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="77860-122">Markeer elke gebeurtenis en zie de resultaatinformatie in het vak onder het tabblad **Algemeen** onder de lijst.</span><span class="sxs-lookup"><span data-stu-id="77860-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
