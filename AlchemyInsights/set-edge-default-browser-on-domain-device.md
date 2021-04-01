---
title: Microsoft Edge instellen als de standaardbrowser op een apparaat dat is verbonden met een domein
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491440"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="f06cf-102">Microsoft Edge instellen als de standaardbrowser op een apparaat dat is verbonden met een domein</span><span class="sxs-lookup"><span data-stu-id="f06cf-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="f06cf-103">Stel Microsoft Edge in als de standaardbrowser:</span><span class="sxs-lookup"><span data-stu-id="f06cf-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="f06cf-104">[Maak een standaardconfiguratiebestand voor associaties](https://go.microsoft.com/fwlink/?linkid=2132437) en sla het lokaal of in een netwerk delen op.</span><span class="sxs-lookup"><span data-stu-id="f06cf-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="f06cf-105">Open de groepsbeleidseditor en ga naar **Beheersjablonen voor computerconfiguratie**  >    >  **Windows Components**  >  **Verkenner.**</span><span class="sxs-lookup"><span data-stu-id="f06cf-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="f06cf-106">Selecteer **Een standaardconfiguratiebestand voor associaties instellen.**</span><span class="sxs-lookup"><span data-stu-id="f06cf-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="f06cf-107">Selecteer **Beleidsinstelling** en selecteer **vervolgens Ingeschakeld.**</span><span class="sxs-lookup"><span data-stu-id="f06cf-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="f06cf-108">Voer **onder** Opties de locatie in van het configuratiebestand voor standaardinstellingen en selecteer **OK.**</span><span class="sxs-lookup"><span data-stu-id="f06cf-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
