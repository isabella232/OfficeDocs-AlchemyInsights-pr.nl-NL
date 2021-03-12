---
title: Uitsluitingen configureren voor Microsoft Defender ATP-scan
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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713570"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="35138-102">Uitsluitingen configureren voor Microsoft Defender ATP-scan</span><span class="sxs-lookup"><span data-stu-id="35138-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="35138-103">In het algemeen kunt u bepaalde bestandsextensies en maplocaties uitsluiten van ATP-scans van Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="35138-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="35138-104">U kunt ook uitsluitingen configureren voor bestanden die door bepaalde processen worden geopend.</span><span class="sxs-lookup"><span data-stu-id="35138-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="35138-105">Zie uitsluitingen configureren en valideren op basis van de [bestandsextensie](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) en maplocatie en Uitsluitingen configureren voor bestanden die worden geopend door processen voor [meer informatie.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="35138-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="35138-106">Zie Microsoft Defender Antivirus-uitsluitingen configureren op Windows Server als u uitsluitingen voor **Windows Server 2016 en 2019** [wilt configureren.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="35138-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="35138-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="35138-107">**Mac**</span></span>

<span data-ttu-id="35138-108">Zie Ondersteunde uitsluitingstypen en De lijst met uitsluitingen configureren voor meer informatie over ondersteunde uitsluitingstypen en het configureren van een lijst [met uitsluitingen voor Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions) [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="35138-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="35138-109">**Opmerking** U kunt ook uitsluitingslijsten valideren met het eicar-testbestand.</span><span class="sxs-lookup"><span data-stu-id="35138-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="35138-110">Zie Uitsluitingslijsten valideren met het [testbestand EI CAR voor meer informatie.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="35138-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="35138-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="35138-111">**Linux**</span></span>

<span data-ttu-id="35138-112">Zie Ondersteunde uitsluitingstypen en Uitsluitingen configureren voor [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) Linux voor meer informatie over ondersteunde [uitsluitingstypen](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)en het configureren van een lijst met uitsluitingen voor Linux.</span><span class="sxs-lookup"><span data-stu-id="35138-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="35138-113">**Opmerking** U kunt ook uitsluitingslijsten valideren met het eicar-testbestand.</span><span class="sxs-lookup"><span data-stu-id="35138-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="35138-114">Zie Uitsluitingslijsten valideren met het [testbestand EI CAR voor meer informatie.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="35138-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 