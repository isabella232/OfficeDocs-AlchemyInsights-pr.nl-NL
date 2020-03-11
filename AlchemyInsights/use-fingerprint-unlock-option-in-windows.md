---
title: Optie voor het ontgrendelen van vingerafdrukken gebruiken in Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588311"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="d63c7-102">Optie voor het ontgrendelen van vingerafdrukken gebruiken in Windows 10</span><span class="sxs-lookup"><span data-stu-id="d63c7-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="d63c7-103">**Windows Hello-vingerafdruk inschakelen**</span><span class="sxs-lookup"><span data-stu-id="d63c7-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="d63c7-104">Als u Windows 10 wilt ontgrendelen met uw vingerafdruk, moet u Windows Hello Fingerprint instellen door windows ten minste één vinger te laten herkennen (windows leren herkennen).</span><span class="sxs-lookup"><span data-stu-id="d63c7-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="d63c7-105">Ga naar **Instellingen >-accounts > aanmeldingsopties** (of klik [hier).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="d63c7-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="d63c7-106">Er worden beschikbare aanmeldingsopties vermeld.</span><span class="sxs-lookup"><span data-stu-id="d63c7-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="d63c7-107">Bijvoorbeeld:</span><span class="sxs-lookup"><span data-stu-id="d63c7-107">For example:</span></span>

    ![Aanmeldingsopties.](media/sign-in-options.png)

2. <span data-ttu-id="d63c7-109">Klik of tik op **Windows Hello Fingerprint**en klik vervolgens op **Instellen**.</span><span class="sxs-lookup"><span data-stu-id="d63c7-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="d63c7-110">Klik in het configuratievenster van Windows Hello op **Aan de slag**.</span><span class="sxs-lookup"><span data-stu-id="d63c7-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="d63c7-111">De vingerafdruksensor wordt geactiveerd en u wordt gevraagd uw vinger op de sensor te plaatsen:</span><span class="sxs-lookup"><span data-stu-id="d63c7-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Vingerafdruksensor.](media/fingerprint-sensor.png)

3. <span data-ttu-id="d63c7-113">Volg de instructies, die u zal vragen om herhaaldelijk uw vinger te scannen.</span><span class="sxs-lookup"><span data-stu-id="d63c7-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="d63c7-114">Wanneer dit is voltooid, hebt u de mogelijkheid om andere vingers toe te voegen die u mogelijk wilt gebruiken voor aanmelding.</span><span class="sxs-lookup"><span data-stu-id="d63c7-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="d63c7-115">De volgende keer dat u zich aanmeldt bij Windows 10, hebt u de mogelijkheid om uw vingerafdruk te gebruiken om dit te doen.</span><span class="sxs-lookup"><span data-stu-id="d63c7-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="d63c7-116">**Windows Hello Fingerprint niet beschikbaar als aanmeldingsoptie**</span><span class="sxs-lookup"><span data-stu-id="d63c7-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="d63c7-117">Als Windows Hello Fingerprint niet wordt weergegeven als optie in **aanmeldingsopties,** betekent dit dat Windows zich niet bewust is van een vingerafdruklezer/scanner die aan uw pc is gekoppeld, of dat een systeembeleid het gebruik ervan voorkomt (als uw pc bijvoorbeeld door uw werkplek wordt beheerd).</span><span class="sxs-lookup"><span data-stu-id="d63c7-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="d63c7-118">Ga als nog maar uit de problemen:</span><span class="sxs-lookup"><span data-stu-id="d63c7-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="d63c7-119">Selecteer de knop **Start** op de taakbalk en zoek naar **Apparaatbeheer**.</span><span class="sxs-lookup"><span data-stu-id="d63c7-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="d63c7-120">Klik of tik om **Apparaatbeheer**te openen.</span><span class="sxs-lookup"><span data-stu-id="d63c7-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="d63c7-121">Vouw in Apparaatbeheer biometrische apparaten uit door op de chevron te klikken.</span><span class="sxs-lookup"><span data-stu-id="d63c7-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrische apparaten.](media/biometric-devices.png)

4. <span data-ttu-id="d63c7-123">Uw vingerafdrukscanner moet worden vermeld als een biometrisch apparaat, zoals de Synaptics WBDI-scanner:</span><span class="sxs-lookup"><span data-stu-id="d63c7-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrische apparaten.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="d63c7-125">Als uw vingerafdrukscanner niet wordt weergegeven en de scanner is geïntegreerd in uw pc, gaat u naar de website van de pc-fabrikant.</span><span class="sxs-lookup"><span data-stu-id="d63c7-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="d63c7-126">Zoek in de sectie technische ondersteuning voor uw pc-model naar een Windows 10-stuurprogramma voor een scanner die u installeren.</span><span class="sxs-lookup"><span data-stu-id="d63c7-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="d63c7-127">Als de scanner gescheiden is van de pc (aangesloten via USB), ga dan naar de website van de scannerfabrikant om Windows 10-apparaatstuurprogrammasoftware te vinden en te installeren voor het scannermodel dat u hebt.</span><span class="sxs-lookup"><span data-stu-id="d63c7-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
