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
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="7294b-102">Windows Memory Diagnostics uitvoeren in Windows 10</span><span class="sxs-lookup"><span data-stu-id="7294b-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="7294b-103">Als Windows en apps op uw pc crashen, vastvriezen of instabiel werken, hebt u mogelijk een probleem met het geheugen (RAM) van de pc.</span><span class="sxs-lookup"><span data-stu-id="7294b-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="7294b-104">U kunt de Windows Memory Diagnostic uitvoeren om te controleren op problemen met het RAM-geheugen van de pc.</span><span class="sxs-lookup"><span data-stu-id="7294b-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="7294b-105">Typ in het zoekvak op de taakbalk **geheugendiagnose** en selecteer **vervolgens Windows Memory Diagnostic**.</span><span class="sxs-lookup"><span data-stu-id="7294b-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="7294b-106">Als u de diagnose wilt uitvoeren, moet de pc opnieuw worden gestart.</span><span class="sxs-lookup"><span data-stu-id="7294b-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="7294b-107">U hebt de optie om direct opnieuw te starten (sla uw werk op en sluit eerst documenten en e-mailberichten) of plan de diagnostische test automatisch uit te voeren wanneer de pc de volgende keer opnieuw wordt gestart:</span><span class="sxs-lookup"><span data-stu-id="7294b-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows Memory Diagnostic](media/windows-memory-diagnostic.png)

<span data-ttu-id="7294b-109">Wanneer de pc opnieuw wordt gestart, wordt het **Windows Memory Diagnostics Tool** automatisch uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="7294b-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="7294b-110">Status en voortgang worden weergegeven terwijl de diagnostische gegevens worden uitgevoerd en u kunt de diagnostische gegevens annuleren door op de **ESC-toets** op het toetsenbord te drukken.</span><span class="sxs-lookup"><span data-stu-id="7294b-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="7294b-111">Wanneer de diagnostische gegevens zijn voltooid, start Windows normaal.</span><span class="sxs-lookup"><span data-stu-id="7294b-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="7294b-112">Direct na het opnieuw opstarten, wanneer het bureaublad wordt  weergegeven, wordt er een melding weergegeven (naast het pictogram Actiecentrum op de taakbalk) om aan te geven of er geheugenfouten zijn gevonden.</span><span class="sxs-lookup"><span data-stu-id="7294b-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="7294b-113">Bijvoorbeeld:</span><span class="sxs-lookup"><span data-stu-id="7294b-113">For example:</span></span>

<span data-ttu-id="7294b-114">Hier ziet u het pictogram Actiecentrum:</span><span class="sxs-lookup"><span data-stu-id="7294b-114">Here's the Action Center icon:</span></span> ![Pictogram Actiecentrum](media/action-center-icon.png) 

<span data-ttu-id="7294b-116">En een voorbeeldmelding:</span><span class="sxs-lookup"><span data-stu-id="7294b-116">And a sample notification:</span></span> ![Geen geheugenfouten](media/no-memory-errors.png)

<span data-ttu-id="7294b-118">Als u de melding hebt  gemist, kunt u het pictogram Actiecentrum op de taakbalk selecteren om het **Actiecentrum** weer te geven en een schuifbare lijst met meldingen te zien.</span><span class="sxs-lookup"><span data-stu-id="7294b-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="7294b-119">Als u gedetailleerde informatie wilt bekijken, **typt u gebeurtenis** in het zoekvak op de taakbalk en selecteert u **Gebeurtenisviewer**.</span><span class="sxs-lookup"><span data-stu-id="7294b-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="7294b-120">Ga in **het linkerdeelvenster** van eventviewer naar **Windows Logs > System.**</span><span class="sxs-lookup"><span data-stu-id="7294b-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="7294b-121">Scan in het rechterdeelvenster de lijst terwijl  u naar de kolom Bron kijkt, totdat u gebeurtenissen ziet met Bronwaarde **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="7294b-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="7294b-122">Markeer elke dergelijke gebeurtenis en bekijk de resultaatgegevens in het vak onder **het** tabblad Algemeen onder de lijst.</span><span class="sxs-lookup"><span data-stu-id="7294b-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
