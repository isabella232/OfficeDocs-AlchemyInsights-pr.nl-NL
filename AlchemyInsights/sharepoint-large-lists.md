---
title: Grote lijsten van SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720128"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="dc838-102">Werken met grote lijsten en bibliotheken in SharePoint</span><span class="sxs-lookup"><span data-stu-id="dc838-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="dc838-103">SharePoint-lijsten en-bibliotheken kunnen 30.000.000-items bevatten, maar wanneer ze meer dan 5.000 items hebben, ziet u mogelijk een foutmelding voor de lijstweergave wanneer u probeert te werken.</span><span class="sxs-lookup"><span data-stu-id="dc838-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="dc838-104">Deze drempelwaarde is ingesteld om de prestaties van de service te kunnen handhaven.</span><span class="sxs-lookup"><span data-stu-id="dc838-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="dc838-105">Deze waarde kan niet worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="dc838-105">It can't be changed.</span></span> <span data-ttu-id="dc838-106">Om te voorkomen dat u dit drempel doet:</span><span class="sxs-lookup"><span data-stu-id="dc838-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="dc838-107">**Modern gebruiken**</span><span class="sxs-lookup"><span data-stu-id="dc838-107">**Use modern**</span></span>

<span data-ttu-id="dc838-108">Weergaven met een groot aantal items werken het best in de moderne ervaring.</span><span class="sxs-lookup"><span data-stu-id="dc838-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="dc838-109">[Gebruik de moderne ervaring](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) om fouten te voorkomen die kunnen optreden in de klassieke weergave.</span><span class="sxs-lookup"><span data-stu-id="dc838-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="dc838-110">**Indexen toevoegen**</span><span class="sxs-lookup"><span data-stu-id="dc838-110">**Add indexes**</span></span>

<span data-ttu-id="dc838-111">Wanneer u op een kolom filtert of sorteert die geen index bevat, wordt er mogelijk een foutbericht weergegeven.</span><span class="sxs-lookup"><span data-stu-id="dc838-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="dc838-112">Handmatig [een index toevoegen](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) uit **lijst instellingen** in het menu instellingen en vervolgens **geïndexeerde kolommen**.</span><span class="sxs-lookup"><span data-stu-id="dc838-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="dc838-113">**De lijstweergave bewerken**</span><span class="sxs-lookup"><span data-stu-id="dc838-113">**Edit the list view**</span></span>

<span data-ttu-id="dc838-114">Als er een fout optreedt wanneer u met een grote lijst werkt, [bewerkt u de lijstweergave](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="dc838-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="dc838-115">Bij de volgende vier wijzigingen worden drempel fouten voor lijstweergave verwijderd.</span><span class="sxs-lookup"><span data-stu-id="dc838-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="dc838-116">Maak alle vier wijzigingen om alle fouten te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="dc838-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="dc838-117">Als u nog steeds fouten krijgt, schakelt u het selectievakje [grote lijsten en bibliotheken beheren](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)in.</span><span class="sxs-lookup"><span data-stu-id="dc838-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="dc838-118">Selecteer **geen** van beide **eerst sorteren op kolom** en **sorteer vervolgens op de kolom**.</span><span class="sxs-lookup"><span data-stu-id="dc838-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="dc838-119">Selecteer **geen** van beide **eerst groeperen op de kolom** en **vervolgens groeperen op de kolom**.</span><span class="sxs-lookup"><span data-stu-id="dc838-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="dc838-120">Selecteer **geen** voor alle kolommen in het gedeelte **Totalen** .</span><span class="sxs-lookup"><span data-stu-id="dc838-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="dc838-121">De selectie van alle kolommen, maar één kolom in de sectie **kolommen** opheffen.</span><span class="sxs-lookup"><span data-stu-id="dc838-121">Deselect all but one column for display from the **Columns** section.</span></span>

