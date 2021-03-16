---
title: De achtergrondservice voor Microsoft Search in Bing verwijderen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816125"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="d2b76-102">De achtergrondservice voor Microsoft Search in Bing verwijderen</span><span class="sxs-lookup"><span data-stu-id="d2b76-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="d2b76-103">Als u de achtergrondservice voor Microsoft Search in Bing wilt verwijderen, kunt u de volgende oplossingen proberen:</span><span class="sxs-lookup"><span data-stu-id="d2b76-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="d2b76-104">Ga als volgt te werk om terug te keren naar de oorspronkelijke instellingen van de zoekmachine:</span><span class="sxs-lookup"><span data-stu-id="d2b76-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="d2b76-105">a.</span><span class="sxs-lookup"><span data-stu-id="d2b76-105">a.</span></span> <span data-ttu-id="d2b76-106">Schakel de **wisselknop Bing gebruiken als standaardzoekmachine [uit.](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**</span><span class="sxs-lookup"><span data-stu-id="d2b76-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="d2b76-107">b.</span><span class="sxs-lookup"><span data-stu-id="d2b76-107">b.</span></span> <span data-ttu-id="d2b76-108">[Ga naar het Microsoft 365-beheercentrum](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) en leeg de instelling die van invloed is op alle gebruikers in uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="d2b76-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="d2b76-109">Als u de achtergrondservice van een afzonderlijk apparaat wilt verwijderen, moet u de volgende taken uitvoeren:</span><span class="sxs-lookup"><span data-stu-id="d2b76-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="d2b76-110">a.</span><span class="sxs-lookup"><span data-stu-id="d2b76-110">a.</span></span> <span data-ttu-id="d2b76-111">Kies **Configuratiescherm > Programma's > programma's en functies**.</span><span class="sxs-lookup"><span data-stu-id="d2b76-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="d2b76-112">b.</span><span class="sxs-lookup"><span data-stu-id="d2b76-112">b.</span></span> <span data-ttu-id="d2b76-113">Klik met de rechtermuisknop **op Microsoft Search in Bing** onder de lijst met geïnstalleerde programma's en klik vervolgens op **Verwijderen.**</span><span class="sxs-lookup"><span data-stu-id="d2b76-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="d2b76-114">Als u de achtergrondservice van meerdere apparaten in uw organisatie wilt verwijderen, meld u zich aan als beheerder en voer u de volgende opdracht uit in een script:</span><span class="sxs-lookup"><span data-stu-id="d2b76-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
