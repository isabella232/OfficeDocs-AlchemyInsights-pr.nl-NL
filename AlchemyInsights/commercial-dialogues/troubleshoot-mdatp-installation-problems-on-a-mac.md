---
title: Problemen met MDATP-installatie op een Mac oplossen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744658"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="e6b19-102">Problemen met MDATP-installatie op een Mac oplossen</span><span class="sxs-lookup"><span data-stu-id="e6b19-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="e6b19-103">Als handmatige installatie mislukt, wordt op **de pagina** Overzicht van de installatiewizard de volgende fout weergegeven:</span><span class="sxs-lookup"><span data-stu-id="e6b19-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="e6b19-104">'Er is een fout opgetreden tijdens de installatie.</span><span class="sxs-lookup"><span data-stu-id="e6b19-104">"An error occurred during installation.</span></span> <span data-ttu-id="e6b19-105">Bij het installatieprogramma is een fout opgetreden waardoor de installatie is mislukt.</span><span class="sxs-lookup"><span data-stu-id="e6b19-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="e6b19-106">Neem contact op met de softwarefabrikant voor hulp.</span><span class="sxs-lookup"><span data-stu-id="e6b19-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="e6b19-107">Voor MDM-implementaties wordt op de pagina ook een algemene installatiefout weergegeven.</span><span class="sxs-lookup"><span data-stu-id="e6b19-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="e6b19-108">Hoewel er geen exacte fouten worden weergegeven voor eindgebruikers, bewaren we een logboekbestand met de voortgang van de installatie, in **/Library/Logs/Microsoft/mdatp/install.log.**</span><span class="sxs-lookup"><span data-stu-id="e6b19-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="e6b19-109">Elke installatiesessie wordt toegevoegd aan dit logboekbestand.</span><span class="sxs-lookup"><span data-stu-id="e6b19-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="e6b19-110">Als u alleen de laatste installatiesessie wilt uitvoeren, gebruikt u `sed` .</span><span class="sxs-lookup"><span data-stu-id="e6b19-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="e6b19-111">Zie Installatieproblemen oplossen [voor Microsoft Defender ATP voor Mac voor](https://go.microsoft.com/fwlink/?linkid=2144615)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="e6b19-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
