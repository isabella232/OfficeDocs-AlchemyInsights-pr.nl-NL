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
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="e539e-102">Berichten herstellen die vastzitten in het postvak uit</span><span class="sxs-lookup"><span data-stu-id="e539e-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="e539e-103">We raden u aan eerst het scenario ['Ik heb problemen met het verzenden, ontvangen of vinden van e-mailberichten'](https://aka.ms/SaRA-OutlookSendReceive) uit te voeren vanuit het hulpprogramma [Microsoft Support and Recovery Assistant.](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="e539e-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="e539e-104">Wanneer een bericht vast komt te zitten in uw postvak IN, is de meest waarschijnlijke oorzaak een grote bijlage of is de optie 'Onmiddellijk verzenden wanneer verbonden' niet ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="e539e-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="e539e-105">**De grote bijlage verwijderen**</span><span class="sxs-lookup"><span data-stu-id="e539e-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="e539e-106">Selecteer in Outlook **Offline verzenden / Ontvangen** > **van werk**.</span><span class="sxs-lookup"><span data-stu-id="e539e-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="e539e-107">Selecteer **Uitvak**in het navigatiedeelvenster .</span><span class="sxs-lookup"><span data-stu-id="e539e-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="e539e-108">Vanaf hier u:</span><span class="sxs-lookup"><span data-stu-id="e539e-108">From here, you can:</span></span> 
    - <span data-ttu-id="e539e-109">Verwijder het bericht (selecteer het bericht en selecteer **Verwijderen).**</span><span class="sxs-lookup"><span data-stu-id="e539e-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="e539e-110">Sleep het bericht naar de map Concepten, dubbelklik om het te openen en verwijder de bijlage selecteer het bericht en selecteer **Verwijderen**).</span><span class="sxs-lookup"><span data-stu-id="e539e-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="e539e-111">Als u een fout ontvangt waarin staat dat Outlook probeert het bericht te verzenden, sluit u Outlook.</span><span class="sxs-lookup"><span data-stu-id="e539e-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="e539e-112">Het kan even duren voordat je het afgaat.</span><span class="sxs-lookup"><span data-stu-id="e539e-112">It may take a few moments to exit.</span></span> <span data-ttu-id="e539e-113">Als Outlook niet wordt gesloten, drukt u op Ctrl+Alt+Verwijderen en selecteert **u Taakbeheer starten**.</span><span class="sxs-lookup"><span data-stu-id="e539e-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="e539e-114">Selecteer in Taakbeheer het tabblad **Processen,** scrol omlaag naar outlook.exe en selecteer **Proces beëindigen**.</span><span class="sxs-lookup"><span data-stu-id="e539e-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="e539e-115">Nadat Outlook is gesloten, start u het opnieuw op en herhaalt u stap 2 en 3.</span><span class="sxs-lookup"><span data-stu-id="e539e-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="e539e-116">Nadat u de bijlage hebt verwijderd, klikt u op Werk verzenden **/ ontvangen** > **offline** om verder te werken online.</span><span class="sxs-lookup"><span data-stu-id="e539e-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="e539e-117">Berichten komen ook vast te zitten in het postvak UIT wanneer u op **Verzenden**klikt, maar u bent niet verbonden.</span><span class="sxs-lookup"><span data-stu-id="e539e-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="e539e-118">Klik **op Verzenden / Ontvangen** en kijk op de knop Offline **werken.**</span><span class="sxs-lookup"><span data-stu-id="e539e-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="e539e-119">Als het blauw is, wordt de verbinding verbroken.</span><span class="sxs-lookup"><span data-stu-id="e539e-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="e539e-120">Klik erop om verbinding te maken (de knop wordt wit) en klik op **Alles verzenden**.</span><span class="sxs-lookup"><span data-stu-id="e539e-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="e539e-121">**Verzenden onmiddellijk inschakelen wanneer deze is aangesloten**</span><span class="sxs-lookup"><span data-stu-id="e539e-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="e539e-122">Klik op het tabblad Bestand op **Opties**.</span><span class="sxs-lookup"><span data-stu-id="e539e-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="e539e-123">Klik in het dialoogvenster Outlook-opties op **Geavanceerd**.</span><span class="sxs-lookup"><span data-stu-id="e539e-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="e539e-124">Klik in de sectie Verzenden en ontvangen om verzenden onmiddellijk in te schakelen **wanneer deze is verbonden.**</span><span class="sxs-lookup"><span data-stu-id="e539e-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="e539e-125">Klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="e539e-125">Click **OK**.</span></span>
 
<span data-ttu-id="e539e-126">Zie voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="e539e-126">For full details, see:</span></span>
- [<span data-ttu-id="e539e-127">Video: Een vastgelopen e-mail verzenden of verwijderen</span><span class="sxs-lookup"><span data-stu-id="e539e-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="e539e-128">E-mail blijft in de map Outbox totdat u handmatig een verzend-/ontvangstbewerking in Outlook start</span><span class="sxs-lookup"><span data-stu-id="e539e-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
