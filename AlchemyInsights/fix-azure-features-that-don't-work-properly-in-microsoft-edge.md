---
title: Wat u moet doen als Azure-functies niet goed werken in Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583307"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="56006-102">Wat u moet doen als Azure-functies niet goed werken in Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="56006-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="56006-103">Microsoft Edge bevat [bekende problemen](https://go.microsoft.com/fwlink/?linkid=2140608) die zijn gerelateerd aan beveiligingszones en van invloed kunnen zijn op hoe Azure gebruikers zich aanmelden bij het Windows-Beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="56006-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="56006-104">Als u problemen ondervindt bij het gebruiken van Azure-functies met Microsoft Edge, voert u de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="56006-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="56006-105">Selecteer in het **Start** menu de **optie Internet opties** en selecteer deze.</span><span class="sxs-lookup"><span data-stu-id="56006-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="56006-106">Ga in het dialoogvenster **Internet eigenschappen** naar het tabblad **beveiliging** .</span><span class="sxs-lookup"><span data-stu-id="56006-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="56006-107">Selecteer de zone **vertrouwde websites** en selecteer vervolgens de knop **sites** .</span><span class="sxs-lookup"><span data-stu-id="56006-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="56006-108">In het dialoogvenster **vertrouwde websites** voegt u de gateway-URL en [https://login.microsoftonline.com](https://login.microsoftonline.com) en [https://login.live.com](https://login.live.com) selecteert u vervolgens **sluiten**.</span><span class="sxs-lookup"><span data-stu-id="56006-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="56006-109">Ga naar het tabblad **Privacy** in het dialoogvenster **Internet eigenschappen** .</span><span class="sxs-lookup"><span data-stu-id="56006-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="56006-110">Selecteer in de sectie **pop-upblokkering** de optie **instellingen**.</span><span class="sxs-lookup"><span data-stu-id="56006-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="56006-111">In het dialoogvenster dat wordt geopend, voegt u de gateway-URL en [https://login.microsoftonline.com](https://login.microsoftonline.com) en [https://login.live.com](https://login.live.com) selecteert u vervolgens **sluiten**.</span><span class="sxs-lookup"><span data-stu-id="56006-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
