---
title: Kan 2010 goedkeuringsworkflow niet toevoegen
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748679"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="a04b0-102">Kan 2010 goedkeuringsworkflow niet toevoegen</span><span class="sxs-lookup"><span data-stu-id="a04b0-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="a04b0-103">In een Microsoft SharePoint-siteverzameling u een globaal herbruikbare werkstroom (zoals ' goedkeuring-SharePoint 2010 ') niet toevoegen aan een lijst of bibliotheek.</span><span class="sxs-lookup"><span data-stu-id="a04b0-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="a04b0-104">Voer de volgende stappen uit om dit probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="a04b0-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="a04b0-105">Open de hoofdwebsite van de siteverzameling in SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="a04b0-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="a04b0-106">Onder **site objecten**, selecteer **Werkstromen**.</span><span class="sxs-lookup"><span data-stu-id="a04b0-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="a04b0-107">Selecteer in de sectie **Nieuw** van het lint **Werkstromen** **herbruikbare werkstroom**.</span><span class="sxs-lookup"><span data-stu-id="a04b0-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="a04b0-108">Voer op het formulier **herbruikbare werkstroom maken** de naam \* \* *Repair2010* \* \* in.</span><span class="sxs-lookup"><span data-stu-id="a04b0-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="a04b0-109">Voor **platform type**, klikt u op **SharePoint 2010 workflow**en klik vervolgens op **OK**.</span><span class="sxs-lookup"><span data-stu-id="a04b0-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="a04b0-110">In de **Opslaan** sectie van de **werkstroom** lint, selecteer **publiceren**.</span><span class="sxs-lookup"><span data-stu-id="a04b0-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="a04b0-111">In de **beheren** sectie van de **werkstroom** lint, selecteer **wereldwijd publiceren**.</span><span class="sxs-lookup"><span data-stu-id="a04b0-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="a04b0-112">Selecteer **OK**in het bevestigingsdialoogvenster dat verschijnt.</span><span class="sxs-lookup"><span data-stu-id="a04b0-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="a04b0-113">Zoek in een webbrowser de hoofdwebsite van de siteverzameling en vervolgens toegang tot site- **instellingen** \> **siteverzameling functies**.</span><span class="sxs-lookup"><span data-stu-id="a04b0-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="a04b0-114">Schakel de functie **workflows** uit:</span><span class="sxs-lookup"><span data-stu-id="a04b0-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="a04b0-115">· Als de functie is *geactiveerd* , klikt u op **deactiveren** en vervolgens op **activeren**.</span><span class="sxs-lookup"><span data-stu-id="a04b0-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="a04b0-116">· Als de functie is *gedeactiveerd* , klikt u op **activeren**.</span><span class="sxs-lookup"><span data-stu-id="a04b0-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="a04b0-117">Raadpleeg het volgende [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="a04b0-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

