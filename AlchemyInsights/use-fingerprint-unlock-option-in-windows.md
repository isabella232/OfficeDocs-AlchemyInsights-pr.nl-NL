---
title: De optie voor het ontgrendelen van vingerafdrukken gebruiken in Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795239"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="c4001-102">De optie voor het ontgrendelen van vingerafdrukken gebruiken in Windows 10</span><span class="sxs-lookup"><span data-stu-id="c4001-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="c4001-103">**Windows hello-vingerafdruk inschakelen**</span><span class="sxs-lookup"><span data-stu-id="c4001-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="c4001-104">Als u Windows 10 wilt ontgrendelen met behulp van uw vingerafdruk, moet u de vingerafdruk van Windows hello instellen door het toevoegen (laat Windows leren herkend) ten minste één vinger.</span><span class="sxs-lookup"><span data-stu-id="c4001-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="c4001-105">Ga naar **instellingen > Accounts > aanmeldingsopties** (of Klik [hier](ms-settings:signinoptions?activationSource=GetHelp).)</span><span class="sxs-lookup"><span data-stu-id="c4001-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="c4001-106">De beschikbare aanmeldingsopties worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="c4001-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="c4001-107">Bijvoorbeeld:</span><span class="sxs-lookup"><span data-stu-id="c4001-107">For example:</span></span>

    ![Aanmeldingsopties.](media/sign-in-options.png)

2. <span data-ttu-id="c4001-109">Klik of tik op de **vingerafdruk van Windows hello**en klik vervolgens op **instellen**.</span><span class="sxs-lookup"><span data-stu-id="c4001-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="c4001-110">Klik in het venster Windows hello instellen op **aan de slag**.</span><span class="sxs-lookup"><span data-stu-id="c4001-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="c4001-111">De vingerafdruksensor wordt geactiveerd, waarna u wordt gevraagd uw vinger op de sensor te plaatsen:</span><span class="sxs-lookup"><span data-stu-id="c4001-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Vingerafdruksensor.](media/fingerprint-sensor.png)

3. <span data-ttu-id="c4001-113">Volg de instructies om u te vragen uw vinger herhaaldelijk te scannen.</span><span class="sxs-lookup"><span data-stu-id="c4001-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="c4001-114">Wanneer dit is gebeurd, kunt u nog andere vingers toevoegen die u mogelijk wilt gebruiken om u aan te melden.</span><span class="sxs-lookup"><span data-stu-id="c4001-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="c4001-115">De volgende keer dat u zich aanmeldt bij Windows 10, kunt u uw vingerafdruk ook gebruiken.</span><span class="sxs-lookup"><span data-stu-id="c4001-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="c4001-116">**De vingerafdruk van Windows hello is niet beschikbaar als aanmeldingsoptie**</span><span class="sxs-lookup"><span data-stu-id="c4001-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="c4001-117">Als u de vingerafdruk van Windows Hello niet als optie **ziet, betekent**dit dat Windows niet op de hoogte is van een vingerafdruklezer/scanner die is aangesloten op uw PC, of dat een systeembeleid het gebruik ervan verhindert (als uw pc bijvoorbeeld wordt beheerd door uw werk).</span><span class="sxs-lookup"><span data-stu-id="c4001-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="c4001-118">Problemen oplossen:</span><span class="sxs-lookup"><span data-stu-id="c4001-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="c4001-119">Selecteer de knop **Start** op de taakbalk en zoek **Apparaatbeheer**.</span><span class="sxs-lookup"><span data-stu-id="c4001-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="c4001-120">Klik of tik om **Apparaatbeheer**te openen.</span><span class="sxs-lookup"><span data-stu-id="c4001-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="c4001-121">Vouw in Apparaatbeheer de biometrische apparaten uit door te klikken op de dubbele punthaak.</span><span class="sxs-lookup"><span data-stu-id="c4001-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrische apparaten.](media/biometric-devices.png)

4. <span data-ttu-id="c4001-123">De vingerafdrukscanner moet als een biometrisch apparaat worden weergegeven, zoals de Synaptics WBDI-scanner:</span><span class="sxs-lookup"><span data-stu-id="c4001-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrische apparaten.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="c4001-125">Ga naar de website van de fabrikant van de PC als de vingerafdrukscanner niet wordt weergegeven en de scanner is geïntegreerd in uw PC.</span><span class="sxs-lookup"><span data-stu-id="c4001-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="c4001-126">Zoek in de sectie technische ondersteuning voor uw PC-model naar een Windows 10-stuurprogramma voor een scanner die u kunt installeren.</span><span class="sxs-lookup"><span data-stu-id="c4001-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="c4001-127">Als de scanner losstaat van de PC (aangesloten via USB), gaat u naar de website van de scannerfabrikant om Windows 10-stuurprogrammasoftware te zoeken en te installeren voor uw scannermodel.</span><span class="sxs-lookup"><span data-stu-id="c4001-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
