---
title: Inhoud wordt niet weergegeven in de zoekresultaten van SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713125"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="0520a-102">Inhoud wordt niet weergegeven in de zoekresultaten van SharePoint</span><span class="sxs-lookup"><span data-stu-id="0520a-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="0520a-103">Volg deze stappen voor probleemoplossing wanneer verwachte inhoud niet in de zoekresultaten wordt weergegeven:</span><span class="sxs-lookup"><span data-stu-id="0520a-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="0520a-104">Controleer of de **site** die de verwachte inhoud bevat, is ingesteld op toestaan dat inhoud wordt weergegeven in zoekresultaten.</span><span class="sxs-lookup"><span data-stu-id="0520a-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="0520a-105">Volg de stappen in de [inhoud van een site weergeven in zoekresultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="0520a-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="0520a-106">Controleer of de **lijst** of **bibliotheek** die de verwachte inhoud bevat, is ingesteld op toestaan dat inhoud wordt weergegeven in zoekresultaten.</span><span class="sxs-lookup"><span data-stu-id="0520a-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="0520a-107">Volg de stappen in [inhoud van lijsten of bibliotheken weergeven in zoekresultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="0520a-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="0520a-108">Controleer of de pagina, het document of de aangepaste pagina-indeling is gepubliceerd als een **primaire versie.**</span><span class="sxs-lookup"><span data-stu-id="0520a-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="0520a-109">Voer stap 3 in [de zoekfunctie retourneert niet alle resultaten in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="0520a-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="0520a-110">Controleer of de gebruiker **gemachtigd** is om de inhoud weer te geven.</span><span class="sxs-lookup"><span data-stu-id="0520a-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="0520a-111">Volg de stappen in [machtigingsniveaus in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="0520a-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="0520a-112">Als het zoekschema is gewijzigd door een nieuwe beheerde eigenschap toe te voegen, of door een beheerde eigenschap te bewerken, of door een beheerde eigenschap te verwijderen, moet u een verkenning en een nieuwe index aanvragen.</span><span class="sxs-lookup"><span data-stu-id="0520a-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="0520a-113">**Indexeer** de inhoud opnieuw door de stappen te volgen in het [handmatig verkennen en opnieuw indexeren van een site, bibliotheek of lijst](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="0520a-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="0520a-114">Het kan enige tijd duren voordat u de resultaten opnieuw controleert.</span><span class="sxs-lookup"><span data-stu-id="0520a-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="0520a-115">Zie voor meer informatie [inhoud op een site inschakelen om te kunnen zoeken](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="0520a-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
