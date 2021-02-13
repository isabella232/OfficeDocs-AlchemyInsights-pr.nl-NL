---
title: Microsoft Edge toevoegen aan Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194477"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="ef040-102">Microsoft Edge toevoegen aan Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ef040-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="ef040-103">Als u Microsoft Edge voor Windows 10 wilt implementeren, configureren, bewaken en beschermen, moet u het eerst toevoegen aan Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="ef040-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="ef040-104">Intune ondersteunt Microsoft Edge 77 en nieuwere versies.</span><span class="sxs-lookup"><span data-stu-id="ef040-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="ef040-105">Intune detecteert eventuele bestaande installaties van Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="ef040-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="ef040-106">Als Microsoft Edge wordt geïnstalleerd in de gebruikerscontext, wordt de installatie door een systeeminstallatie overschreven in de gebruikerscontext.</span><span class="sxs-lookup"><span data-stu-id="ef040-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="ef040-107">Als Microsoft Edge is geïnstalleerd in de systeemcontext, wordt het installatieproces gerapporteerd.</span><span class="sxs-lookup"><span data-stu-id="ef040-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="ef040-108">Vooraf geïnstalleerde Microsoft Edge 77 en nieuwere versies, voor alle kanalen in gebruikerscontext, worden overschreven met Microsoft Edge geïnstalleerd in systeemcontext.</span><span class="sxs-lookup"><span data-stu-id="ef040-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="ef040-109">**Vereiste**</span><span class="sxs-lookup"><span data-stu-id="ef040-109">**Prerequisite**</span></span>

<span data-ttu-id="ef040-110">Windows 10 versie 1709 of hoger</span><span class="sxs-lookup"><span data-stu-id="ef040-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="ef040-111">**Stappen voor het toevoegen van Edge aan Intune**</span><span class="sxs-lookup"><span data-stu-id="ef040-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="ef040-112">[Configureer de app in Intune.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="ef040-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="ef040-113">[Configureer de app-informatie.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="ef040-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="ef040-114">[De app-instellingen configureren.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="ef040-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="ef040-115">[Selecteer de bereikcodes (optioneel).](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="ef040-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="ef040-116">[Voeg de app toe.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="ef040-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="ef040-117">Zie Probleemoplossing voor [meer hulp.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="ef040-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




