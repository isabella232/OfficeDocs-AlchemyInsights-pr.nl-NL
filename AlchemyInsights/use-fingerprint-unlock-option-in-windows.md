---
title: De optie Vingerafdruk ontgrendelen gebruiken in Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796672"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="2f047-102">De optie Vingerafdruk ontgrendelen gebruiken in Windows 10</span><span class="sxs-lookup"><span data-stu-id="2f047-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="2f047-103">**Windows Hello Fingerprint inschakelen**</span><span class="sxs-lookup"><span data-stu-id="2f047-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="2f047-104">Als u Windows 10 wilt ontgrendelen met uw vingerafdruk, moet u Windows Hello Fingerprint instellen door ten minste één vinger toe te voegen (zodat Windows leert herkennen).</span><span class="sxs-lookup"><span data-stu-id="2f047-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="2f047-105">Ga naar **Instellingen > Accounts > aanmeldingsopties** (of klik [hier).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="2f047-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="2f047-106">Beschikbare aanmeldingsopties worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="2f047-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="2f047-107">Bijvoorbeeld:</span><span class="sxs-lookup"><span data-stu-id="2f047-107">For example:</span></span>

    ![Aanmeldingsopties.](media/sign-in-options.png)

2. <span data-ttu-id="2f047-109">Klik of tik op **Windows Hello Fingerprint** en klik vervolgens op **Instellen.**</span><span class="sxs-lookup"><span data-stu-id="2f047-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="2f047-110">Klik in het windows Hello-installatievenster op **Aan de slag.**</span><span class="sxs-lookup"><span data-stu-id="2f047-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="2f047-111">De vingerafdruk sensor wordt geactiveerd en u wordt gevraagd uw vinger op de sensor te plaatsen:</span><span class="sxs-lookup"><span data-stu-id="2f047-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Vingerafdruk sensor.](media/fingerprint-sensor.png)

3. <span data-ttu-id="2f047-113">Volg de instructies, waarmee u wordt gevraagd uw vinger herhaaldelijk te scannen.</span><span class="sxs-lookup"><span data-stu-id="2f047-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="2f047-114">Wanneer dit is voltooid, kunt u andere vingers toevoegen die u mogelijk wilt gebruiken voor aanmelding.</span><span class="sxs-lookup"><span data-stu-id="2f047-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="2f047-115">De volgende keer dat u zich bij Windows 10 aan melden, hebt u de mogelijkheid om uw vingerafdruk te gebruiken om dit te doen.</span><span class="sxs-lookup"><span data-stu-id="2f047-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="2f047-116">**Windows Hello Fingerprint niet beschikbaar als aanmeldingsoptie**</span><span class="sxs-lookup"><span data-stu-id="2f047-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="2f047-117">Als Windows Hello Fingerprint niet wordt weergegeven als een optie **in** aanmeldingsopties, betekent dit dat Windows niet op de hoogte is van een vingerafdruklezer/scanner die aan uw pc is gekoppeld of dat een systeembeleid het gebruik ervan verhindert (als uw pc bijvoorbeeld wordt beheerd door uw werkplek).</span><span class="sxs-lookup"><span data-stu-id="2f047-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="2f047-118">Problemen oplossen:</span><span class="sxs-lookup"><span data-stu-id="2f047-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="2f047-119">Selecteer de **knop Start** op de taakbalk en zoek **naar Apparaatbeheer.**</span><span class="sxs-lookup"><span data-stu-id="2f047-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="2f047-120">Klik of tik om **Apparaatbeheer te openen.**</span><span class="sxs-lookup"><span data-stu-id="2f047-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="2f047-121">Vouw in Apparaatbeheer biometrische apparaten uit door op de punthaak te klikken.</span><span class="sxs-lookup"><span data-stu-id="2f047-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrische apparaten.](media/biometric-devices.png)

4. <span data-ttu-id="2f047-123">Uw vingerafdrukscanner moet worden weergegeven als een biometrisch apparaat, zoals de Synaptics WBDI-scanner:</span><span class="sxs-lookup"><span data-stu-id="2f047-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrische apparaten.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="2f047-125">Als uw vingerafdrukscanner niet wordt weergegeven en de scanner is geïntegreerd in uw pc, gaat u naar de website van de fabrikant van de pc.</span><span class="sxs-lookup"><span data-stu-id="2f047-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="2f047-126">Zoek in de sectie technische ondersteuning voor uw pc-model naar een Windows 10-stuurprogramma voor een scanner die u kunt installeren.</span><span class="sxs-lookup"><span data-stu-id="2f047-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="2f047-127">Als de scanner is gescheiden van de pc (gekoppeld via USB), gaat u naar de website van de fabrikant van de scanner om de stuurprogrammasoftware van Windows 10 te zoeken en te installeren voor het scannermodel dat u hebt.</span><span class="sxs-lookup"><span data-stu-id="2f047-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
