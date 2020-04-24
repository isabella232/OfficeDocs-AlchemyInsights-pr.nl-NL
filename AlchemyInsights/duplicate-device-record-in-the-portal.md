---
title: Dubbele apparaatrecord in de portal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789684"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="814a0-102">Dubbele apparaatrecord in de portal</span><span class="sxs-lookup"><span data-stu-id="814a0-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="814a0-103">U kunt twee records zien voor een apparaat in de portal als de status van het co-beheer niet correct wordt gerapporteerd voor de site van Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="814a0-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="814a0-104">Voor het controleren van de status van het co-beheer van apparaat, raadpleegt u de kolom **Met co-beheer** van het apparaat in de Configuration Manager-console.</span><span class="sxs-lookup"><span data-stu-id="814a0-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="814a0-105">Als de kolom niet zichtbaar is, kunt u deze toevoegen door met de rechtermuisknop op een van de kolomkoppen te klikken en deze in de lijst te selecteren.</span><span class="sxs-lookup"><span data-stu-id="814a0-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="814a0-106">De waarde Met co-beheer moet **Ja** zijn.</span><span class="sxs-lookup"><span data-stu-id="814a0-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="814a0-107">Als de waarde **Nee** is, opent u de applet Configuration Manager-client op het clientapparaat en controleert u de eigenschap **Co-beheer** op het tabblad Algemeen.</span><span class="sxs-lookup"><span data-stu-id="814a0-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="814a0-108">Als de waarde**Ingeschakeld** is, duidt dit op problemen met clientcommunicatie met het beheerpunt.</span><span class="sxs-lookup"><span data-stu-id="814a0-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="814a0-109">Bekijk **CcmMessaging.log** op het apparaat om mogelijke verbindingsproblemen te onderzoeken.</span><span class="sxs-lookup"><span data-stu-id="814a0-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="814a0-110">Als de waarde **Ingeschakeld** is en het apparaat is geregistreerd bij intune, controleert u of het apparaat het beleid voor co-beheer heeft ontvangen door **CoManagementHandler.log** op het apparaat te bekijken.</span><span class="sxs-lookup"><span data-stu-id="814a0-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
