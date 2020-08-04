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
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="94a59-102">TeamViewer gebruiken om Intune-apparaten op afstand te beheren</span><span class="sxs-lookup"><span data-stu-id="94a59-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="94a59-103">Apparaten die door Intune worden beheerd, kunnen op afstand worden beheerd met [TeamViewer.](https://www.teamviewer.com/)</span><span class="sxs-lookup"><span data-stu-id="94a59-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="94a59-104">Als u Intune wilt beheren met TeamViewer, voert u de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="94a59-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="94a59-105">Begin met het verkrijgen van referenties van TeamViewer om de TeamViewer Connector op Intune in te stellen.</span><span class="sxs-lookup"><span data-stu-id="94a59-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="94a59-106">Hierdoor kan de beheerder referenties invoeren in de Gebruikersinterface van De Verbinder van TeamViewer onder Apparaten, een eenmalige bewerking om de koppeling tussen Intune en de TeamViewer-service tot stand te brengen.</span><span class="sxs-lookup"><span data-stu-id="94a59-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="94a59-107">**Deel 1: Een sessie starten met een extern apparaat**</span><span class="sxs-lookup"><span data-stu-id="94a59-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="94a59-108">Selecteer onder **Alle apparaten**het apparaat waarmee u een externe sessie wilt starten.</span><span class="sxs-lookup"><span data-stu-id="94a59-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="94a59-109">Van **... Meer**, selecteer **Nieuwe hulpsessie op afstand**.</span><span class="sxs-lookup"><span data-stu-id="94a59-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="94a59-110">Selecteer **Ja** om te erkennen dat u een externe sessie wilt instellen.</span><span class="sxs-lookup"><span data-stu-id="94a59-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="94a59-111">Nadat de aanvraag 'Een nieuwe externe sessie starten' is bevestigd door de TeamViewer-service, ziet u een optie om **hulp op afstand** te starten onder de details van het deelvenster Overzicht (of Essentials) voor het apparaat.</span><span class="sxs-lookup"><span data-stu-id="94a59-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="94a59-112">Selecteer **Meer weergeven** om het deelvenster uit te vouwen en de status Hulp op afstand weer te geven.</span><span class="sxs-lookup"><span data-stu-id="94a59-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="94a59-113">Selecteer **Externe sessie starten** om de sessie aan de beheerderszijde te starten.</span><span class="sxs-lookup"><span data-stu-id="94a59-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="94a59-114">Kies ervoor om de binaire TeamViewer (Windows) te downloaden en selecteer **Uitvoeren**.</span><span class="sxs-lookup"><span data-stu-id="94a59-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="94a59-115">**Opmerking** U elke webbrowserpagina negeren die is geopend voor de TeamViewer-website.</span><span class="sxs-lookup"><span data-stu-id="94a59-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="94a59-116">Bevestig het verzoek aan de TeamViewer-app om wijzigingen aan te brengen op het apparaat (alleen Windows).</span><span class="sxs-lookup"><span data-stu-id="94a59-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="94a59-117">De TeamViewer-app wordt gestart en bevat de sessiecode om de verbinding met het externe apparaat te verifiëren.</span><span class="sxs-lookup"><span data-stu-id="94a59-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="94a59-118">**Deel 2: Op het apparaat dat wordt gericht op een externe sessie**</span><span class="sxs-lookup"><span data-stu-id="94a59-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="94a59-119">Open het bedrijfsportaal in Intune.</span><span class="sxs-lookup"><span data-stu-id="94a59-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="94a59-120">Zoek naar een meldingsvlag: 'Uw IT-beheerder vraagt de controle over dit apparaat aan voor een hulpsessie op afstand' en selecteer de melding.</span><span class="sxs-lookup"><span data-stu-id="94a59-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="94a59-121">Kies ervoor om de TeamViewer-toepassing te downloaden of de download van de TeamViewer-app te bevestigen in de app Store en selecteer **Uitvoeren**.</span><span class="sxs-lookup"><span data-stu-id="94a59-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="94a59-122">**Opmerking** U elke webbrowserpagina negeren die is geopend voor de TeamViewer-website.</span><span class="sxs-lookup"><span data-stu-id="94a59-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="94a59-123">Bevestig het verzoek aan de TeamViewer-app om wijzigingen aan te brengen op het apparaat (alleen Windows).</span><span class="sxs-lookup"><span data-stu-id="94a59-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="94a59-124">De TeamViewer-app wordt gestart en bevat de sessiecode om de verbinding met het externe apparaat te verifiëren.</span><span class="sxs-lookup"><span data-stu-id="94a59-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="94a59-125">Een pop-up vraagt of u de sessie wilt laten starten.</span><span class="sxs-lookup"><span data-stu-id="94a59-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="94a59-126">**Opmerking** De sessiecodes die door de TeamViewer-service worden gegenereerd, worden alleen eenmalig gebruikt.</span><span class="sxs-lookup"><span data-stu-id="94a59-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="94a59-127">Als u de verbinding verliest, moet u:</span><span class="sxs-lookup"><span data-stu-id="94a59-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="94a59-128">Sluit de instantie van de TeamViewer-app op het externe apparaat en op het beheerwerkstation.</span><span class="sxs-lookup"><span data-stu-id="94a59-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="94a59-129">Sluit het bedrijfsportaal op het externe apparaat.</span><span class="sxs-lookup"><span data-stu-id="94a59-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="94a59-130">Start een nieuwe "Nieuwe remote Assistance session" vanuit de admin portal.</span><span class="sxs-lookup"><span data-stu-id="94a59-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="94a59-131">Open de bedrijfsportal op het externe apparaat opnieuw om de nieuwe melding te ontvangen.</span><span class="sxs-lookup"><span data-stu-id="94a59-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="94a59-132">Download en open de TeamViewer-app op zowel het externe apparaat als het beheerwerkstation, zoals voorheen.</span><span class="sxs-lookup"><span data-stu-id="94a59-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>