---
title: Uitsluitingen configureren voor Microsoft Defender ATP scannen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543680"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="fe824-102">Uitsluitingen configureren voor Microsoft Defender ATP scannen</span><span class="sxs-lookup"><span data-stu-id="fe824-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="fe824-103">In het algemeen kunt u bepaalde bestandsextensies en maplocaties uitsluiten van Microsoft Defender ATP scans.</span><span class="sxs-lookup"><span data-stu-id="fe824-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="fe824-104">U kunt ook uitsluitingen configureren voor bestanden die door bepaalde processen zijn geopend.</span><span class="sxs-lookup"><span data-stu-id="fe824-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="fe824-105">Zie Uitsluitingen configureren en valideren op basis van [bestandsextensie](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) en maplocatie en Uitsluitingen configureren voor bestanden die door processen zijn geopend voor meer [informatie.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="fe824-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="fe824-106">Zie Uitsluitingen configureren **voor Windows Server 2016 en 2019** Microsoft Defender Antivirus [configureren op Windows Server.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="fe824-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="fe824-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="fe824-107">**Mac**</span></span>

<span data-ttu-id="fe824-108">Zie Ondersteunde uitsluitingstypen en De lijst met uitsluitingen configureren voor meer informatie over ondersteunde uitsluitingstypen en het configureren van een lijst [met uitsluitingen voor Mac.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions) [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="fe824-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="fe824-109">**Opmerking** U kunt ook lijsten met uitsluitingen valideren met het EICAR-testbestand.</span><span class="sxs-lookup"><span data-stu-id="fe824-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="fe824-110">Zie Lijsten met uitsluitingen valideren [met het EICAR-testbestand](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="fe824-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="fe824-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="fe824-111">**Linux**</span></span>

<span data-ttu-id="fe824-112">Zie Ondersteunde uitsluitingstypen en Uitsluitingen configureren voor [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) linux voor meer informatie over ondersteunde [uitsluitingstypen](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)en het configureren en valideren van uitsluitingen voor Microsoft Defender ATP voor Linux.</span><span class="sxs-lookup"><span data-stu-id="fe824-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="fe824-113">**Opmerking** U kunt ook lijsten met uitsluitingen valideren met het EICAR-testbestand.</span><span class="sxs-lookup"><span data-stu-id="fe824-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="fe824-114">Zie Lijsten met uitsluitingen valideren [met het EICAR-testbestand](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="fe824-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 