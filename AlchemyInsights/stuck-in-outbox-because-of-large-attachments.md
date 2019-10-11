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
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="b0a51-102">Berichten herstellen die vastzitten in het postvak uit</span><span class="sxs-lookup"><span data-stu-id="b0a51-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="b0a51-103">Het is raadzaam dat u begint met het uitvoeren van het scenario [' Ik heb problemen met het verzenden, ontvangen of vinden van e-mail berichten '](https://aka.ms/SaRA-OutlookSendReceive) van het hulpprogramma [Microsoft ondersteuning en herstel-assistent](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="b0a51-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="b0a51-104">Wanneer een bericht vastloopt in het postvak uit, zijn de meest waarschijnlijke oorzaken:</span><span class="sxs-lookup"><span data-stu-id="b0a51-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="b0a51-105">Grote bijlagen.</span><span class="sxs-lookup"><span data-stu-id="b0a51-105">Large attachments.</span></span>
- <span data-ttu-id="b0a51-106">De optie **direct verzenden bij verbinding** is niet ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="b0a51-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="b0a51-107">Grote bijlagen verwijderen:</span><span class="sxs-lookup"><span data-stu-id="b0a51-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="b0a51-108">Selecteer in Outlook**offline werk** **verzenden/ontvangen** > .</span><span class="sxs-lookup"><span data-stu-id="b0a51-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="b0a51-109">Selecteer **Postvak**uit in het navigatiedeelvenster.</span><span class="sxs-lookup"><span data-stu-id="b0a51-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="b0a51-110">Vanaf hier u:</span><span class="sxs-lookup"><span data-stu-id="b0a51-110">From here, you can:</span></span> 
    - <span data-ttu-id="b0a51-111">Verwijder het bericht (Selecteer het en selecteer vervolgens **verwijderen**).</span><span class="sxs-lookup"><span data-stu-id="b0a51-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="b0a51-112">Sleep het bericht naar de map concepten, dubbelklik erop om het te openen en verwijder de bijlage Selecteer deze en selecteer vervolgens **verwijderen**).</span><span class="sxs-lookup"><span data-stu-id="b0a51-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="b0a51-113">Als er een foutbericht wordt weergegeven dat Outlook probeert te verzenden, sluit u Outlook.</span><span class="sxs-lookup"><span data-stu-id="b0a51-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="b0a51-114">Het kan enkele ogenblikken duren om af te sluiten.</span><span class="sxs-lookup"><span data-stu-id="b0a51-114">It may take a few moments to exit.</span></span> <span data-ttu-id="b0a51-115">Als Outlook niet wordt gesloten, drukt u op CTRL + ALT + DELETE en selecteert u **Taakbeheer starten**.</span><span class="sxs-lookup"><span data-stu-id="b0a51-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="b0a51-116">Selecteer in Taakbeheer het tabblad **processen** , Scrol omlaag naar Outlook. exe en selecteer **proces beëindigen**.</span><span class="sxs-lookup"><span data-stu-id="b0a51-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="b0a51-117">Nadat Outlook is gesloten, start u het opnieuw en herhaalt u stap 2 en 3.</span><span class="sxs-lookup"><span data-stu-id="b0a51-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="b0a51-118">Nadat u de bijlage hebt verwijderd, klikt u op**offline werk** **verzenden/ontvangen** > om online te gaan werken.</span><span class="sxs-lookup"><span data-stu-id="b0a51-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="b0a51-119">Berichten komen ook vast te zitten in het postvak uit wanneer u op **verzenden**klikt, maar u bent niet verbonden.</span><span class="sxs-lookup"><span data-stu-id="b0a51-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="b0a51-120">Klik op **verzenden/ontvangen** en Bekijk de knop **offline werken** .</span><span class="sxs-lookup"><span data-stu-id="b0a51-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="b0a51-121">Als dit blauw is, wordt de verbinding verbroken.</span><span class="sxs-lookup"><span data-stu-id="b0a51-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="b0a51-122">Selecteer deze om verbinding te maken (de knop wordt wit) en klik op **Alles verzenden**.</span><span class="sxs-lookup"><span data-stu-id="b0a51-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="b0a51-123">De optie **direct verzenden inschakelen wanneer deze is aangesloten**:</span><span class="sxs-lookup"><span data-stu-id="b0a51-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="b0a51-124">Selecteer **Bestands** > **Opties** >  **Geavanceerd**.</span><span class="sxs-lookup"><span data-stu-id="b0a51-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="b0a51-125">Selecteer in de sectie **verzenden en ontvangen** de optie **direct verzenden wanneer deze is verbonden**en kies vervolgens **OK**.</span><span class="sxs-lookup"><span data-stu-id="b0a51-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="b0a51-126">Zie voor de volledige details:</span><span class="sxs-lookup"><span data-stu-id="b0a51-126">For full details see:</span></span>
- [<span data-ttu-id="b0a51-127">Video: een vastgelopen e-mail bericht verzenden of verwijderen</span><span class="sxs-lookup"><span data-stu-id="b0a51-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="b0a51-128">E-mail blijft in de map Postvak uit totdat u handmatig een bewerking voor verzenden/ontvangen in Outlook start</span><span class="sxs-lookup"><span data-stu-id="b0a51-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
