---
title: Hulp bij de instelling voor het nachtlampje
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404398"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="379b8-102">Hulp bij de instelling voor het nachtlampje</span><span class="sxs-lookup"><span data-stu-id="379b8-102">Help with the night light display setting</span></span>

<span data-ttu-id="379b8-103">Zie Uw beeldscherm instellen voor [nachttijd in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)voor meer informatie over de weergave-instellingen voor nacht.</span><span class="sxs-lookup"><span data-stu-id="379b8-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="379b8-104">Als de opties voor nachtlamp grijs worden weergegeven in Instellingen, controleert u het beeldschermdrijf:</span><span class="sxs-lookup"><span data-stu-id="379b8-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="379b8-105">Klik op het zoekvak op de taakbalk en typ **Apparaatbeheer** en selecteer **vervolgens Apparaatbeheer** in de zoekresultaten.</span><span class="sxs-lookup"><span data-stu-id="379b8-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="379b8-106">Vouw **Beeldschermadapters uit.**</span><span class="sxs-lookup"><span data-stu-id="379b8-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="379b8-107">Helaas is de nachtlampfunctie niet beschikbaar als uw apparaat een DisplayLink-stuurprogramma of een Basic Display-stuurprogramma gebruikt.</span><span class="sxs-lookup"><span data-stu-id="379b8-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="379b8-108">De nachtlampfunctie maakt gebruik van recente grafische technologie, dus mogelijk moet u uw beeldschermdrijf bijwerken:</span><span class="sxs-lookup"><span data-stu-id="379b8-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="379b8-109">Controleer op updates door naar **Instellingen bijwerken starten**  >  **&**  >  **Windows**  >  **Update** controleren  >  **op updates**.</span><span class="sxs-lookup"><span data-stu-id="379b8-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="379b8-110">OF</span><span class="sxs-lookup"><span data-stu-id="379b8-110">OR</span></span>

- <span data-ttu-id="379b8-111">Ga naar de ondersteuningswebsite van de hardwarefabrikant om handmatig de nieuwste weergave-stuurprogramma's te downloaden en te installeren.</span><span class="sxs-lookup"><span data-stu-id="379b8-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="379b8-112">Nachtlamp opnieuw instellen in het register</span><span class="sxs-lookup"><span data-stu-id="379b8-112">Reset night light in the registry</span></span>

<span data-ttu-id="379b8-113">Als het bijwerken van het beeldscherm stuurprogramma niet werkt, moet u mogelijk nachtlamp opnieuw instellen in het register.</span><span class="sxs-lookup"><span data-stu-id="379b8-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="379b8-114">**Let op:** Deze stap voor probleemoplossing wordt alleen aanbevolen voor geavanceerde gebruikers.</span><span class="sxs-lookup"><span data-stu-id="379b8-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="379b8-115">Er kunnen ernstige problemen optreden als u het register onjuist wijzigt.</span><span class="sxs-lookup"><span data-stu-id="379b8-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="379b8-116">Voor extra beveiliging maakt u een back-up van het register voordat u het wijzigt, zodat u het kunt herstellen als er problemen optreden.</span><span class="sxs-lookup"><span data-stu-id="379b8-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="379b8-117">Typ **regedit** in het zoekvak en selecteer **registereditor** in de zoekresultaten.</span><span class="sxs-lookup"><span data-stu-id="379b8-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="379b8-118">Ga naar de volgende registersleutel:</span><span class="sxs-lookup"><span data-stu-id="379b8-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="379b8-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="379b8-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="379b8-120">De volgende subsleutel exporteren en verwijderen:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="379b8-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="379b8-121">De volgende subsleutel exporteren en verwijderen:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="379b8-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="379b8-122">Start Windows opnieuw en controleer of de opties voor nachtlamp beschikbaar zijn.</span><span class="sxs-lookup"><span data-stu-id="379b8-122">Restart Windows and verify if the night light options are available.</span></span>


