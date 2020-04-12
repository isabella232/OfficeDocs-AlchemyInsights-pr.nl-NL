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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232625"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="cad32-102">Berichten herstellen die vastzitten in het postvak uit</span><span class="sxs-lookup"><span data-stu-id="cad32-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="cad32-103">We raden u aan eerst het scenario ['Ik heb problemen met het verzenden, ontvangen of vinden van e-mailberichten'](https://aka.ms/SaRA-OutlookSendReceive) uit te voeren vanuit het hulpprogramma [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) op de betreffende machine.</span><span class="sxs-lookup"><span data-stu-id="cad32-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="cad32-104">Wanneer een bericht vast komt te zitten in uw postvak IN, is de meest waarschijnlijke oorzaak een grote bijlage of is de optie 'Onmiddellijk verzenden wanneer verbonden' niet ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="cad32-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="cad32-105">**De grote bijlage verwijderen**</span><span class="sxs-lookup"><span data-stu-id="cad32-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="cad32-106">Klik **op Werk verzenden / ontvangen** > **offline**.</span><span class="sxs-lookup"><span data-stu-id="cad32-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="cad32-107">Klik in het navigatiedeelvenster op **Uitvak**.</span><span class="sxs-lookup"><span data-stu-id="cad32-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="cad32-108">Vanaf hier u:</span><span class="sxs-lookup"><span data-stu-id="cad32-108">From here, you can:</span></span> 
    - <span data-ttu-id="cad32-109">Verwijder het bericht.</span><span class="sxs-lookup"><span data-stu-id="cad32-109">Delete the message.</span></span> <span data-ttu-id="cad32-110">Selecteer deze en klik op **Verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="cad32-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="cad32-111">Sleep het bericht naar de **conceptmap,** dubbelklik om het bericht te openen en verwijder de bijlage (klik erop en klik op **Verwijderen).**</span><span class="sxs-lookup"><span data-stu-id="cad32-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="cad32-112">Als een fout aangeeft dat Outlook probeert het bericht te verzenden, sluit u Outlook.</span><span class="sxs-lookup"><span data-stu-id="cad32-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="cad32-113">Het kan even duren voordat je het afgaat.</span><span class="sxs-lookup"><span data-stu-id="cad32-113">It may take a few moments to exit.</span></span> <span data-ttu-id="cad32-114">Als Outlook niet wordt gesloten, drukt u op **Ctrl+Alt+Verwijderen** en klikt u op **Taakbeheer starten**.</span><span class="sxs-lookup"><span data-stu-id="cad32-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="cad32-115">Selecteer in Taakbeheer het tabblad **Processen,** scrol omlaag naar outlook.exe en klik op **Proces beëindigen**.</span><span class="sxs-lookup"><span data-stu-id="cad32-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="cad32-116">Nadat Outlook is gesloten, start u Outlook opnieuw op en herhaalt u stap 2-3.</span><span class="sxs-lookup"><span data-stu-id="cad32-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="cad32-117">Nadat u de bijlage hebt verwijderd, klikt u op Werk verzenden **/ ontvangen** > **offline** om de knop uit te kiezen en om verder te werken online.</span><span class="sxs-lookup"><span data-stu-id="cad32-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="cad32-118">Berichten komen ook vast te zitten in het postvak UIT wanneer u op **Verzenden**klikt, maar u bent niet verbonden.</span><span class="sxs-lookup"><span data-stu-id="cad32-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="cad32-119">Klik **op Verzenden / Ontvangen** en kijk op de knop Offline **werken.**</span><span class="sxs-lookup"><span data-stu-id="cad32-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="cad32-120">Als het blauw is, wordt de verbinding verbroken.</span><span class="sxs-lookup"><span data-stu-id="cad32-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="cad32-121">Klik erop om verbinding te maken (de knop wordt wit) en klik op **Alles verzenden**.</span><span class="sxs-lookup"><span data-stu-id="cad32-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="cad32-122">**Verzenden onmiddellijk inschakelen wanneer deze is aangesloten**</span><span class="sxs-lookup"><span data-stu-id="cad32-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="cad32-123">Klik op het tabblad Bestand op **Opties**.</span><span class="sxs-lookup"><span data-stu-id="cad32-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="cad32-124">Klik in het dialoogvenster Outlook-opties op **Geavanceerd**.</span><span class="sxs-lookup"><span data-stu-id="cad32-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="cad32-125">Klik in de sectie Verzenden en ontvangen om verzenden onmiddellijk in te schakelen **wanneer deze is verbonden.**</span><span class="sxs-lookup"><span data-stu-id="cad32-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="cad32-126">Klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="cad32-126">Click **OK**.</span></span>
 
<span data-ttu-id="cad32-127">Zie voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="cad32-127">For full details, see:</span></span>
- [<span data-ttu-id="cad32-128">Video: Een vastgelopen e-mail verzenden of verwijderen</span><span class="sxs-lookup"><span data-stu-id="cad32-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="cad32-129">E-mail blijft in de map Outbox totdat u handmatig een verzend-/ontvangstbewerking in Outlook start</span><span class="sxs-lookup"><span data-stu-id="cad32-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
