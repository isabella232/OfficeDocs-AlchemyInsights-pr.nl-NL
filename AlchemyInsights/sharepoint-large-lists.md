---
title: Grote SharePoint-lijsten
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488512"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="a66ac-102">Werken met grote lijsten en bibliotheken in SharePoint</span><span class="sxs-lookup"><span data-stu-id="a66ac-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="a66ac-103">SharePoint-lijsten en-bibliotheken kunnen maximaal 30.000.000 items bevatten, maar als ze meer dan 5.000 items hebben, ziet u mogelijk een drempel fout voor de lijstweergave wanneer u ermee probeert te werken.</span><span class="sxs-lookup"><span data-stu-id="a66ac-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="a66ac-104">Deze drempelwaarde is van plaats om de prestaties van de service te behouden.</span><span class="sxs-lookup"><span data-stu-id="a66ac-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="a66ac-105">Het kan niet worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="a66ac-105">It can't be changed.</span></span> <span data-ttu-id="a66ac-106">Om te voorkomen dat het raken van deze drempel:</span><span class="sxs-lookup"><span data-stu-id="a66ac-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="a66ac-107">**Gebruik moderne**</span><span class="sxs-lookup"><span data-stu-id="a66ac-107">**Use modern**</span></span>

<span data-ttu-id="a66ac-108">Weergaven met veel items werken het beste in de moderne ervaring.</span><span class="sxs-lookup"><span data-stu-id="a66ac-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="a66ac-109">[Gebruik de moderne ervaring](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) om fouten te voorkomen die u zien in de klassieke ervaring.</span><span class="sxs-lookup"><span data-stu-id="a66ac-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="a66ac-110">**Indexen toevoegen**</span><span class="sxs-lookup"><span data-stu-id="a66ac-110">**Add indexes**</span></span>

<span data-ttu-id="a66ac-111">Wanneer u filtert of sorteert op een kolom die geen index heeft, ziet u mogelijk een foutbericht.</span><span class="sxs-lookup"><span data-stu-id="a66ac-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="a66ac-112">[Voeg een index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) handmatig toe vanuit de **lijst instellingen** in het menu instellingen en klik vervolgens op **geïndexeerde kolommen**.</span><span class="sxs-lookup"><span data-stu-id="a66ac-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="a66ac-113">**De lijstweergave bewerken**</span><span class="sxs-lookup"><span data-stu-id="a66ac-113">**Edit the list view**</span></span>

<span data-ttu-id="a66ac-114">Als er een fout optreedt bij het werken met een grote lijst, bewerkt u de [Lijstweergave](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="a66ac-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="a66ac-115">Met de volgende vier wijzigingen worden drempel fouten voor lijstweergave verwijderd.</span><span class="sxs-lookup"><span data-stu-id="a66ac-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="a66ac-116">Maak alle vier wijzigingen om alle fouten te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="a66ac-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="a66ac-117">Als u nog steeds fouten krijgt, controleert u [grote lijsten en bibliotheken beheren](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="a66ac-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="a66ac-118">Selecteer **geen** van beide **eerst sorteren op de kolom** en **vervolgens sorteren op de kolom**.</span><span class="sxs-lookup"><span data-stu-id="a66ac-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="a66ac-119">Selecteer **geen** van beide **eerste groep op de kolom** en **vervolgens groeperen op de kolom**.</span><span class="sxs-lookup"><span data-stu-id="a66ac-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="a66ac-120">Selecteer **geen** voor alle kolommen in de sectie **Totalen** .</span><span class="sxs-lookup"><span data-stu-id="a66ac-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="a66ac-121">Hef de selectie van alle één kolom op voor weergave in het gedeelte **kolommen** .</span><span class="sxs-lookup"><span data-stu-id="a66ac-121">Deselect all but one column for display from the **Columns** section.</span></span>

