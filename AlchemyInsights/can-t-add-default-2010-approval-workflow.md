---
title: Geen standaard toevoegen goedkeuringswerkstroom 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28283625"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="cceff-102">Geen standaard toevoegen goedkeuringswerkstroom 2010</span><span class="sxs-lookup"><span data-stu-id="cceff-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="cceff-103">In een siteverzameling van Microsoft SharePoint niet kunt u een globaal herbruikbare werkstroom (bijvoorbeeld "goedkeuring - SharePoint 2010") toevoegen aan een lijst of bibliotheek.</span><span class="sxs-lookup"><span data-stu-id="cceff-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="cceff-104">Dit probleem oplossen door de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="cceff-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="cceff-105">Open de website van de hoofdmap van de siteverzameling in SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="cceff-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="cceff-106">Selecteer onder **Site-objecten**, **werkstromen**.</span><span class="sxs-lookup"><span data-stu-id="cceff-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="cceff-107">Selecteer in de sectie **Nieuw** van het lint **werkstromen** **Herbruikbare werkstroom**.</span><span class="sxs-lookup"><span data-stu-id="cceff-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="cceff-p101">Voer de naam van het formulier **Herbruikbare werkstroom maken** \* \*\*Repair2010\*\*\*. **SharePoint 2010-werkstroom**te selecteren voor het **Type Platform**en klik vervolgens op **OK**.</span><span class="sxs-lookup"><span data-stu-id="cceff-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="cceff-110">Selecteer in de sectie van het lint **Workflow** **Opslaan** **publiceren**.</span><span class="sxs-lookup"><span data-stu-id="cceff-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="cceff-p102">Selecteer in de sectie **beheren** van het lint voor de **werkstroom** **Globaal publiceren**. Klik in het dialoogvenster bevestiging op **OK**.</span><span class="sxs-lookup"><span data-stu-id="cceff-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="cceff-p103">In een webbrowser en Ga naar de website van de hoofdmap van de siteverzameling en vervolgens naar **Site-instellingen** \> **Onderdelen van de siteverzameling**. Vervolgens de functie voor **werkstromen** schakelen:</span><span class="sxs-lookup"><span data-stu-id="cceff-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="cceff-115">· Als de functie *geactiveerd is* , klikt u op **deactiveren,** en klik op **activeren**.</span><span class="sxs-lookup"><span data-stu-id="cceff-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="cceff-116">· Als de functie *gedeactiveerd is* , klikt u op **activeren**.</span><span class="sxs-lookup"><span data-stu-id="cceff-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="cceff-117">Raadpleeg het volgende [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="cceff-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

