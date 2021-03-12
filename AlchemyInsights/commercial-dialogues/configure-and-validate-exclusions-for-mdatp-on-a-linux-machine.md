---
title: Uitsluitingen configureren en valideren voor MDATP op een Linux-computer
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744538"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="03225-102">Uitsluitingen configureren en valideren voor MDATP op een Linux-computer</span><span class="sxs-lookup"><span data-stu-id="03225-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="03225-103">U kunt bepaalde bestanden, mappen, processen en proces geopende bestanden uitsluiten van MDATP-scans.</span><span class="sxs-lookup"><span data-stu-id="03225-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="03225-104">Uitsluitingen helpen voorkomen dat software en bestanden die uniek of aangepast zijn aan uw organisatie, onjuist worden gedetecteerd.</span><span class="sxs-lookup"><span data-stu-id="03225-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="03225-105">Uitsluitingen helpen ook bij het beperken van prestatieproblemen die worden veroorzaakt door MDATP.</span><span class="sxs-lookup"><span data-stu-id="03225-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="03225-106">Zie Uitsluitingen [configureren en valideren voor MDATP voor Linux voor meer informatie.](https://go.microsoft.com/fwlink/?linkid=2144517)</span><span class="sxs-lookup"><span data-stu-id="03225-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="03225-107">De uitsluitingen die in dit artikel worden beschreven, zijn niet van toepassing op andere mogelijkheden van MDATP voor Linux, waaronder eindpuntdetectie en -antwoord (EDR).</span><span class="sxs-lookup"><span data-stu-id="03225-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="03225-108">Bestanden die u uitsluit met de methoden die in dit artikel worden beschreven, kunnen nog steeds EDR-waarschuwingen en andere detectiemogelijkheden activeren.</span><span class="sxs-lookup"><span data-stu-id="03225-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
