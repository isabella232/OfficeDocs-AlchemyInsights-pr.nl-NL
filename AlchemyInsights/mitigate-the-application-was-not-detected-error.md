---
title: Corrigeren van de fout De applicatie is niet gedetecteerd
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810479"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="28c5e-102">Corrigeren van de fout 'De applicatie is niet gedetecteerd'</span><span class="sxs-lookup"><span data-stu-id="28c5e-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="28c5e-103">De door Intune gemelde app-installatiefout 'De applicatie is niet gedetecteerd nadat de installatie is voltooid', kan optreden bij alle belangrijke besturingssystemen (Windows, iOS en Android).</span><span class="sxs-lookup"><span data-stu-id="28c5e-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="28c5e-104">De meest voorkomende scenario's die deze fout veroorzaken, zijn onder meer:</span><span class="sxs-lookup"><span data-stu-id="28c5e-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="28c5e-105">De app is na de eerste implementatie buiten Intune bijgewerkt (vanuit een app-store van derden).</span><span class="sxs-lookup"><span data-stu-id="28c5e-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="28c5e-106">Sommige toepassingen, zoals Google Chrome, voeren mogelijk automatische updates uit.</span><span class="sxs-lookup"><span data-stu-id="28c5e-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="28c5e-107">Een gebruiker heeft de app verwijderd na de eerste installatie.</span><span class="sxs-lookup"><span data-stu-id="28c5e-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="28c5e-108">U kunt dit probleem corrigeren door eerst een revisie uit te voeren van de betrokken apparaten, om te bepalen welk scenario de fout veroorzaakt.</span><span class="sxs-lookup"><span data-stu-id="28c5e-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="28c5e-109">Als de app is bijgewerkt buiten Intune, kunt u de app-implementatie zo instellen dat de toepassingsversie wordt genegeerd.</span><span class="sxs-lookup"><span data-stu-id="28c5e-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="28c5e-110">Hiertoe stelt u onder **App-configuratie > App-informatie** de optie **App-versie negeren** in op **Ja**.</span><span class="sxs-lookup"><span data-stu-id="28c5e-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="28c5e-111">Bij de communicatie met uw klant kan het handig zijn om de toepassing te promoten als 'vereist', om er zo voor te zorgen dat de nieuwste versie wordt geïmplementeerd.</span><span class="sxs-lookup"><span data-stu-id="28c5e-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="28c5e-112">Het is ook mogelijk om op het iOS-platform de functionaliteit van **AutoUpdate** te gebruiken die is gekoppeld aan het Apple Volume Purchase Program. Dit kan zo worden ingesteld dat deze automatisch wordt bijgewerkt naar nieuwe toepassingsversies zodra deze beschikbaar komen.</span><span class="sxs-lookup"><span data-stu-id="28c5e-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="28c5e-113">Voor meer informatie over het oplossen van problemen met de installatie van apps, raadpleegt u [problemen met het installeren van apps.</span><span class="sxs-lookup"><span data-stu-id="28c5e-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
